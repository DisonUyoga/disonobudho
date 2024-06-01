+++
categories = ["web-dev"]
coders = ["DisonObudho"]
date = 2023-11-19T23:00:00Z
description = "FullStack Responsive Real Estate Site Using React and Nodejs"
github = ["https://github.com/DisonUyoga/mern-real-estate-site.git"]
image = "https://cdn.svgporn.com/logos/nodejs.svg"
title = "React and Nodejs"
type = "post"
[[tech]]
logo = "https://cdn.svgporn.com/logos/nodejs.svg"
name = "React and Nodejs Rest Framework"
url = "https://real-estate-site-7a20.onrender.com/"


+++

## React Public Site Link:

[Real Estate Website](https://real-estate-site-7a20.onrender.com/)

The following react depencies were used in this project:

     "@emailjs/browser": "^3.11.0",
    "@reduxjs/toolkit": "^1.9.7",
    "animate.css": "^4.1.1",
    "aos": "^2.3.4",
    "axios": "^1.6.2",
    "bootstrap": "^5.3.2",
    "date-fn": "^0.0.2",
    "dotenv": "^16.3.1",
    "firebase": "^10.7.0",
    "framer-motion": "^10.16.5",
    "react": "^18.2.0",
    "react-carousel": "^4.3.0",
    "react-dom": "^18.2.0",
    "react-icons": "^4.12.0",
    "react-leaflet": "^4.2.1",
    "react-loaders": "^3.0.1",
    "react-redux": "^8.1.3",
    "react-router-dom": "^6.20.0",
    "react-toastify": "^9.1.3",
    "reactstrap": "^9.2.1",
    "redux-persist": "^6.0.0",
    "remixicon": "^3.6.0",
    "sass": "^1.69.5",
    "slick-carousel": "^1.8.1",
    "swiper": "^11.0.5",
    "tw-elements": "^1.0.0"

## Sections

### Homepage

![Homepage Screenshot](https://res.cloudinary.com/dfjpdzsin/image/upload/loggedinhomepage_kgeovq.png "Homepage Screenshot")

The avatar on the navbar is only visible when the user is signed.

### Sign up

![sign up](https://res.cloudinary.com/dfjpdzsin/image/upload/signin_kdue2h.png "signup Screenshot")

Firebase has been used to implement google login logic to enhance user experience

### Profile

![profile Screenshot](https://res.cloudinary.com/dfjpdzsin/image/upload/profile_t8zhjk.png "profile Screenshot")

I have invested on the power of react state management using `useEffect` and `useState` to efficiently update profile photo before submiting to the backend. To enhance user experience, once the user updates the profile photo, the changes take effect before actual backend response.

I have skillfully utilized firebase storage api to upload avatar before responding with a url that is later stored as a string in the mongodb.

![listing Screenshot](https://res.cloudinary.com/dfjpdzsin/image/upload/listings_meniq7.png "listing Screenshot")

Once logged in, a user can perform all the CRUD operations and can only view their listing.

#### node implementation

A token created using the user id;

```bash
const token =jwt.sign({id:validUser._id}, process.env.JWT_SECRET)

const {password:pass,...rest}=validUser._doc
res.cookie("access_token", token, {httpOnly:true, expires: new Date(Date.now()+24*60*60*1000)}).status(200).json(rest)
```

Is accessed via a middleware;

```bash
export const verifyToken=(req, res,next)=>{
const token =req.cookies.access_token
console.log(token)
if(!token) return next(errorHandler(401, "Unauthorized"))
jwt.verify(token, process.env.JWT_SECRET,(err,user)=>{
  if(err) return next(errorHandler(403, "Forbidden"))
  req.user=user
  next()
})

}
```

To ensure that a user only edits or view their own listing.

### Search

![](https://res.cloudinary.com/dfjpdzsin/image/upload/estatesearch_ui5bjn.png)

I have invested heavily in the power of search params and mongoose operators to develop a powerful search engine, without using powerful search libraries such as `algolia`, which is economical for smaller projects.

# Installation

## React

### Cloning the site

To clone the project, ensure you have git installed

```bash
git clone https://github.com/DisonUyoga/mern-real-estate-site.git
```

##### frontend

```bash
cd mern-real-estate-site/client
```

```bash
npm i
```

```bash
npm run dev
```

#### backend

```bash
cd mern-real-estate-site
```

```bash
npm i
```

```bash
npm start
```
