+++
categories = ["web-dev"]
coders = []
date = 2020-06-19T23:00:00Z
description = "Responsive Ecommerce website"
github = ["https://github.com/DisonUyoga/Advance-Ecommerce-Furniture-site.git"]
image = "https://cdn.svgporn.com/logos/react.svg"
title = "Responsive Ecommerce Website"
type = "post"
[[tech]]
logo = "https://cdn.svgporn.com/logos/react.svg"
name = "React"
url = "https://mainafurnitures.vercel.app/"


+++

### Click the link to Take a Tour into the site

[React Ecommerce Site](https://mainafurnitures.vercel.app/)

The following depencies were used in this project:

    "@reduxjs/toolkit": "^1.9.7",
    "@testing-library/jest-dom": "^6.1.4",
    "animate.css": "^4.1.1",
    "axios": "^1.5.1",
    "bootstrap": "^5.3.2",
    "bootstrap-icons": "^1.11.1",
    "date-fn": "^0.0.2",
    "firebase": "^10.5.0",
    "framer-motion": "^10.16.4",
    "jquery": "^3.7.1",
    "loaders.css": "^0.1.2",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-floating-whatsapp": "^5.0.8",
    "react-leaflet": "^4.2.1",
    "react-loaders": "^3.0.1",
    "react-redux": "^8.1.3",
    "react-router": "^6.17.0",
    "react-router-dom": "^6.17.0",
    "react-toastify": "^9.1.3",
    "reactstrap": "^9.2.0",
    "remixicon": "^3.5.0",
    "sass": "^1.69.5",
    "tw-elements": "^1.0.0",
    "web-vitals": "^3.5.0"

## Sections

### Homepage

![Homepage Screenshot](https://res-console.cloudinary.com/dfjpdzsin/media_explorer_thumbnails/fe91837d84272623c2804fd387183e13/detailed "Homepage Screenshot")
![Homepage Screenshot](https://res-console.cloudinary.com/dfjpdzsin/media_explorer_thumbnails/1e17890ab957f51bf8e0cfa70e6e4904/detailed "Homepage Screenshot")

I have used the power of useRef and useState react hooks and pure css to develop a responsive navbar. To optimize user experience, I have used css sticky property to ensure easy user navigation. I have used @keyframes with raw css to create beautiful animation in the navbar.

### Shop

![Shop Screenshot](https://res-console.cloudinary.com/dfjpdzsin/media_explorer_thumbnails/f34d84156f91cad537d0d24262312894/detailed "Shop Screenshot")

The main focus in this page is to optimize user experience by establishing powerfull search engine using simple javascript code. the main methods used are:

- `filter`
- `map`
- `icontains`

The primary goal was to optimize user experience using simple code from javascript without using powerful search libraries such as Algolia.

Howerver, I managed to achieve this using redux to maintain state

### Card

![Card Screenshot](https://res-console.cloudinary.com/dfjpdzsin/media_explorer_thumbnails/8c6378e1905d3e0de183632ffb21cd34/detailed "Card Screenshot")

This card is bult with pure css, `framer-motion` and remixicons to create beatiful animation when hovering. The UI is higly responsive.

### Cart

![](https://res-console.cloudinary.com/dfjpdzsin/media_explorer_thumbnails/578cec3dedbf738c7a2cf559a389893a/detailed)

The cart automatically calculate the total amount of cart. Items can also be deleted from the cart. More importantly. Raw css has been used to make the UI highly responsive

## Installation

### Cloning the site

To clone the project, ensure you have git installed

```bash
git clone https://github.com/DisonUyoga/Advance-Ecommerce-Furniture-site.git
```

```bash
cd Advance-Ecommerce-Furniture-site
```

```bash
npm i
```

```bash
npm run dev
```
