[Readme.txt](https://github.com/user-attachments/files/34699006/Readme.txt)
# Travel Around Sri Lanka

A responsive, single-page travel website that showcases popular tourist destinations in Sri Lanka. It features a full-screen video hero, animated destination cards, an about section, a contact form and a 3D testimonial slider.

## Features

- **Video hero section** with a dark overlay and an animated "liquid drop" glass navigation bar
- **Destination cards** with hover lift, image zoom and scroll-triggered fade-up animations (pure CSS, no JavaScript)
- **About section** with a background image and overlay
- **Contact form** powered by Formspree (no backend needed)
- **Testimonial slider** with a 3D coverflow effect, autoplay, pagination and navigation arrows (Swiper)
- **Social media buttons** with a liquid fill hover effect
- **Fully responsive** layout for desktop, tablet and mobile
- Smooth scrolling between sections from the navigation bar

## Sections

| Section | Description |
|---|---|
| Home | Background video, headline and Explore button |
| Destination | Cards for Sigiriya, Ella Nine Arch, Mirissa, Galle Fort, Yala, Temple of the Tooth, Dambulla, Horton Plains and Arugam Bay |
| About | Introduction to the travel guide |
| Contact | Contact form with name, email and message |
| Testimonials | 3D slider with traveller reviews |

## Built With

- HTML5
- CSS3 (Flexbox, `backdrop-filter`, CSS animations, scroll-driven animations)
- JavaScript (Swiper initialisation)
- [Swiper](https://swiperjs.com/) v11 for the testimonial slider
- [Remix Icon](https://remixicon.com/) for stars and arrows
- [Font Awesome](https://fontawesome.com/) for social media icons
- [Google Fonts](https://fonts.google.com/): Montserrat and Unbounded
- [Formspree](https://formspree.io/) for the contact form

## Project Structure

```
project-folder/
├── index.html
├── style.css
├── script.js
├── README.md
├── assets/
│   └── arrow_icon.png
└── img/
    ├── Home-Banner.webm
    ├── sigiriya.jpg
    ├── ella.jpg
    ├── mirissa.jpg
    ├── galle.jpg
    ├── yala.jpg
    ├── maligawa.jpg
    ├── dambulla.jpg
    ├── hortain.jpg
    ├── arugam.jpg
    ├── about_img.jpg
    ├── home-img-1.png
    ├── home-img-2.png
    └── pp1.jpeg ... pp5.jpeg
```

## Getting Started

1. Download or clone the project.
2. Make sure the `img/` and `assets/` folders contain the images and video listed above.
3. Open `index.html` in your browser. No build step or installation is needed.

An internet connection is required for the CDN libraries (Swiper, Remix Icon, Font Awesome) and Google Fonts.

## Customisation

- **Hero video:** replace `img/Home-Banner.webm` with your own video.
- **Destinations:** copy a `.card` block inside `.card_container` in `index.html`, then change the image, title and description.
- **Overlay darkness:** adjust the `rgba(...)` values in `.hero_overlay`, `.About_section` and `.testimonial` in `style.css`.
- **Colours:** the main accent colours are `#ff8a00` (orange) and `#f2ff00` (yellow).
- **Contact form:** create a form at [formspree.io](https://formspree.io/) and replace the URL in the form's `action` attribute in `index.html` with your own endpoint.
- **Testimonials:** copy an `<article class="testimonial__card swiper-slide">` block inside `.swiper-wrapper` and edit the name, photo and review.

## Browser Support

Works in the latest versions of Chrome, Edge, Brave, Firefox and Safari.

The scroll-triggered fade-up animations use CSS scroll-driven animations (`animation-timeline: view()`). Browsers that do not support this feature simply show the content without the animation.

## Author

Created by **[Your Name]**.

## License

This project is for learning and personal use. Add a license of your choice if you plan to share or publish it.
