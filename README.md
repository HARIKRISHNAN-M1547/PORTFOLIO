# Harikrishnan M | Portfolio

Personal portfolio website of **Harikrishnan M**, a final-year B.Tech Electronics and Communication Engineering student at SNGCET, Payyanur, focused on embedded systems, IoT and robotics.

**Live site:** https://harikrishnan-m1547.github.io

## Features

- **Hero section** with a large auto-scrolling word marquee (EMBEDDED ★ IoT ★ ROBOTICS) behind a cut-out profile photo
- **Robot reveal effect:** hovering over the photo opens a circle that shows a robotic version of the portrait
- **Voice greeting:** a short hello plays while the reveal is open (tap to play and stop on touch screens)
- **Typing animation** in the hero headline
- **About section** with a "Listen to my intro" audio button and a resume download
- **Project cards** with angled corners: NEPTUNE underwater ROV, Mushroom Cultivation System, Rescue Guardian, Battle Bot, Orby
- **Experience and certifications** timeline
- **Contact section** with GitHub, email and LinkedIn links and a message form that opens the visitor's email app
- Scroll-reveal animations, responsive layout for phones and tablets, and support for reduced-motion settings

## Built with

- HTML, CSS and vanilla JavaScript (single `index.html`, no frameworks or build step)
- Google Fonts: Archivo and Space Grotesk
- Hosted on GitHub Pages

## Project structure

```
.
├── index.html
├── README.md
├── images/
│   ├── profile.png        # background-removed portrait (hero)
│   ├── profile-alt.png    # robotic version, same size and pose (reveal effect)
│   └── about.png          # photo for the About section
├── audio/
│   ├── hello.mp3          # hero voice greeting (optional)
│   └── about.mp3          # About-section intro (optional)
└── resume/
    └── resume.pdf
```

If an audio file is missing, the browser reads the text aloud instead.

## Run locally

1. Clone the repository:
   ```
   git clone https://github.com/HARIKRISHNAN-M1547/HARIKRISHNAN-M1547.github.io.git
   ```
2. Open the folder in VS Code.
3. Right-click `index.html` and choose **Open with Live Server**, or double-click the file to open it in a browser.

## Customize

| What | Where in `index.html` |
| --- | --- |
| Colors | `:root` variables at the top of the CSS |
| Hero words | the `.words` block |
| Hero headline and typing words | the `.hello` block and `const WORDS=` in the script |
| Reveal circle size | `.photo:hover{--r:30px}` |
| Voice text | `const HELLO=` and `const INTRO=` in the script |
| Projects | the `.cards` section |
| Email and LinkedIn | the Contact section |

## Deploy on GitHub Pages

1. Push the project to a repository on GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select the `main` branch and the `/ (root)` folder, then save.
4. The site goes live after a minute or two.

File names on GitHub are case-sensitive, so keep the names in `images/`, `audio/` and `resume/` exactly as in the code.

## Notes

- Browsers block sound until the visitor has clicked or tapped the page once, so the hover voice may be silent before the first click.
- The robot image must have the same size and pose as `profile.png`, or the reveal will look misaligned.

## Contact

- Email: hari1547santhosh@gmail.com
- LinkedIn: https://www.linkedin.com/in/harikrishnan1547
- GitHub: https://github.com/HARIKRISHNAN-M1547
