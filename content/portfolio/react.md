+++
categories = ["web-dev"]
coders = []
date = 2023-11-19T23:00:00Z
description = "FullStack Responsive Ecommerce website with React and Django Rest"
github = ["https://github.com/DisonUyoga/Advance-Ecommerce-Furniture-site.git", "https://github.com/DisonUyoga/Advanced-ecommerce-furniture-site.git"]
image = "https://cdn.svgporn.com/logos/react.svg"
title = "FullStack Responsive Ecommerce Website"
type = "post"
[[tech]]
logo = "https://cdn.svgporn.com/logos/react.svg"
name = "React and Django Rest Framework"
url = "https://mainafurnitures.vercel.app/"


+++

---

## Responsive Furniture Website

### Project Overview

Developed a modern, responsive furniture website to showcase my proficiency in front-end design, CSS, animations, JavaScript, and React, with backend integration using Django Rest Framework. This project highlights my ability to create aesthetically pleasing, user-friendly interfaces and implement dynamic functionalities for an enhanced user experience.

### Key Features

- **Responsive Design**: Utilized advanced CSS techniques, including Flexbox and Grid, to ensure the site is fully responsive and looks great on all devices.
- **CSS Animations**: Implemented smooth and engaging animations to enhance the visual appeal and interactivity of the site, providing a dynamic user experience.
- **JavaScript & React**: Built the frontend using React to create reusable components, manage state efficiently, and provide a seamless single-page application experience.
- **Django Rest Framework**: Integrated with a Django Rest API to manage backend functionalities, enabling secure and efficient data handling and user authentication.
- **Interactive UI/UX**: Focused on creating an intuitive user interface with easy navigation, product filtering, and interactive elements to improve user engagement.

### Technologies Used

- **Front-end**: HTML5, CSS3, JavaScript (ES6+), React
- **Styling**: CSS Animations, Flexbox, Grid, Sass
- **Back-end**: Django Rest Framework
- **Tools**: Git, Webpack, Babel

### Highlights

- Designed and developed a responsive layout that adapts seamlessly to various screen sizes and devices.
- Created dynamic animations using CSS to provide a visually engaging user experience.
- Developed reusable React components to streamline the development process and ensure code maintainability.
- Implemented secure and efficient data handling using Django Rest Framework for backend integration.

### Outcome

This project demonstrates my ability to combine design aesthetics with functional development to create a responsive and interactive website. The furniture site serves as a testament to my skills in modern web development technologies and my capability to deliver high-quality, user-centric web applications.

---

## Public Site Link:

[React Ecommerce Site](https://mainafurnitures.vercel.app/)

## Django Rest Public API Link:

[API (Django Rest)](https://obudhodison.pythonanywhere.com/api/products/)

The following react depencies were used in this project:

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

![Homepage Screenshot](https://res.cloudinary.com/dfjpdzsin/image/upload/homepage_xyk6it.png "Homepage Screenshot")
![Homepage](https://res.cloudinary.com/dfjpdzsin/image/upload/v1717225383/mobileScreenhomepage_ovhcpn.png "Homepage Screenshot")

I have used the power of useRef and useState react hooks and pure css to develop a responsive navbar. To optimize user experience, I have used css sticky property to ensure easy user navigation. I have used @keyframes with raw css to create beautiful animation in the navbar.

### Shop

![Shop Screenshot](https://res.cloudinary.com/dfjpdzsin/image/upload/v1717222935/mobileshop_wi5e65.png "Shop Screenshot")

The main focus in this page is to optimize user experience by establishing powerfull search engine using simple javascript code. the main methods used are:

- `filter`
- `map`
- `icontains`

The primary goal was to optimize user experience using simple code from javascript without using powerful search libraries such as Algolia.

Howerver, I managed to achieve this using redux to maintain state

### Card

![Card Screenshot](https://res.cloudinary.com/dfjpdzsin/image/upload/v1717222907/homepagecard_j6pcvf.png "Card Screenshot")

This card is bult with pure css, `framer-motion` and remixicons to create beatiful animation when hovering. The UI is higly responsive.

### Cart

![](https://res.cloudinary.com/dfjpdzsin/image/upload/v1717222773/homecart_zv9lce.png)

The cart automatically calculate the total amount of cart. Items can also be deleted from the cart. More importantly. Raw css has been used to make the UI highly responsive

# Installation

## React

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

## Django Rest

```bash
git clone https://github.com/DisonUyoga/Advanced-ecommerce-furniture-site.git
```

```bash
cd Advanced-ecommerce-furniture-site
```

```bash
python install virtualenv venv
```

```bash
cd venv/Scripts/activate
```

```bash
python install -r requirements.txt
```

```bash
python manage.py runserver
```
