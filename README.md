Netflix Landing Page

A front-end replica of a page dedicated to the Stranger Things series, inspired by the Netflix interface.

The project was created using HTML, CSS, and vanilla JavaScript, without external frameworks or libraries.

Features
Hero section with an embedded YouTube video
Information about the series
Trailer carousel
Recommended titles carousel
Forward and backward navigation one item at a time
Trailer playback inside an overlay
Email address validation
Additional information section
Subscription plan section
Footer with informational links
Technologies Used
HTML5
CSS3
JavaScript
YouTube Embed
Project Structure
project/
│
├── index.html
├── style.css
├── script.js
├── README.md
│
├── img/
│   ├── Netflix_2015_logo.svg.png
│   ├── stranger-things-logo.webp
│   ├── storie-dal-1985.webp
│   ├── 7-vite.webp
│   ├── a-list.webp
│   ├── it.webp
│   ├── it-2.webp
│   ├── lockwood.webp
│   ├── lucifer.webp
│   ├── vampire-diaries.webp
│   └── profezia-del-male.webp
│
├── video/
│   ├── video1.mp4
│   ├── video2.mp4
│   ├── video3.mp4
│   ├── video4.mp4
│   ├── video5.mp4
│   └── video6.mp4
│
└── pagina-login/
    └── login.html
How to Run the Project
Download or clone the project.
Make sure the img, video, and pagina-login folders are present.
Open the index.html file in your browser.

No dependencies or server installation are required.

To avoid possible issues when loading local files, you can use the Live Server extension in Visual Studio Code.

Carousels

The page contains two carousels:

a carousel for trailers;
a carousel for recommended titles.

When the < or > arrows are clicked, the content moves by one item at a time.

The trailer carousel displays three items at the same time, while the poster carousel displays six.

The arrows are automatically hidden when the carousel reaches the beginning or the end.

Trailer Playback

When a trailer card is clicked, the video opens inside an overlay above the page.

To close the video, click outside the video player.

While the video is open, page scrolling is temporarily disabled.

Email Validation

The email field in the subscription section is validated using JavaScript.

An error message is displayed when:

the field is empty;
the entered address does not match a valid email format.

Example of a valid email:

name@email.com
Customization
Changing the Number of Visible Items

The following variables are available in the script.js file:

const videoVisibili = 3;
const posterVisibili = 6;

Change these values to modify the number of trailers and posters displayed at the same time.

Adding a New Trailer

Add a new element inside the trailer section:

<div>
    <video src="video/new-video.mp4"></video>
    <p>New trailer</p>
</div>

The video file must be placed inside the video folder.

Adding a New Poster

Add a new element inside the .poster container:

<div>
    <img src="img/new-poster.webp" alt="Content title">
</div>

The image must be placed inside the img folder.

Possible Improvements
Make the page fully responsive
Add animations when the carousels move
Add swipe support for smartphones and tablets
Add carousel position indicators
Improve button accessibility
Add more descriptive alt attributes to images
Replace the arrow elements with <button> elements
Store submitted form data
Connect the page to a back-end
Notes

This project was created for educational purposes only.

Netflix, Stranger Things, the logos, images, and content used belong to their respective owners. This project is not affiliated with, sponsored by, or endorsed by Netflix.
