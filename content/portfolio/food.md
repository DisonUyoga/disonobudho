+++
categories = ["web-dev"]
coders = ["DisonObudho"]
date = 2023-11-19T23:00:00Z
description = "FullStack Responsive Food Delivery website with React and Django Rest"
github = ["https://github.com/DisonUyoga/food_delivery_ecommerce.git", "https://github.com/DisonUyoga/food_backend.git"]
image = "https://cdn.svgporn.com/logos/react.svg"
title = "FullStack Responsive Food Delivery Website"
type = "post"
[[tech]]
logo = "https://cdn.svgporn.com/logos/react.svg"
name = "React and Django Rest Framework"
url = "https://mainafurnitures.vercel.app/"


+++

---

**Project Title: Responsive Food Delivery Web Application**

**Description:**
Developed a responsive web application for a food delivery service, demonstrating expertise in front-end and back-end development. This project showcases my ability to design and implement a modern, user-friendly interface with seamless functionality.

**Key Features:**

- **User Interface Design:** Created an intuitive and visually appealing design using HTML, CSS, and JavaScript, ensuring a cohesive and engaging user experience.
- **Responsive Design:** Implemented responsive design principles using CSS and media queries to ensure the application is accessible and functional across various devices, including desktops, tablets, and smartphones.
- **Interactive Elements:** Enhanced user interactions with dynamic features and animations using JavaScript, providing a smooth and interactive browsing experience.
- **Backend Development:** Utilized Django Rest Framework to build a robust and scalable backend, managing user authentication, order processing, and data storage efficiently.
- **API Integration:** Designed and integrated RESTful APIs to enable smooth communication between the frontend and backend, ensuring real-time updates and data synchronization.

**Technologies Used:**

- Frontend: HTML, CSS, JavaScript, React
- Backend: Django Rest Framework
- Tools: Git, GitHub,

**Outcome:**
The project successfully demonstrates my ability to design and develop a responsive web application from scratch, combining modern front-end technologies with a powerful backend framework. The final product is a fully functional food delivery site that is both user-friendly and efficient.

---

## React Public Site Link:

[Food Delivery Website](https://food-delivery-ecommerce-kyi2.vercel.app/)

## Django Rest Public API Link:

[API (Django Rest)](https://foodbackend.pythonanywhere.com/api/products/)

The following react depencies were used in this project:

    "@reduxjs/toolkit": "^1.9.7",
    "axios": "^1.6.2",
    "bootstrap": "^5.3.2",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-icons": "^4.12.0",
    "react-paginate": "^8.2.0",
    "react-redux": "^8.1.3",
    "react-router-dom": "^6.20.0",
    "react-slick": "^0.29.0",
    "react-toastify": "^9.1.3",
    "reactstrap": "^9.2.1",
    "remixicon": "^3.5.0",
    "sass": "^1.69.5",
    "slick-carousel": "^1.8.1",
    "web-vitals": "^3.5.0"

## Sections

### Homepage

![Homepage Screenshot](https://res.cloudinary.com/dfjpdzsin/image/upload/foodhomepage_jyd4ts.png "Homepage Screenshot")

I have used the power of useRef and useState react hooks and pure css to develop a responsive navbar. To optimize user experience, I have used css sticky property to ensure easy user navigation. I have used @keyframes with raw css to create beautiful animation in the navbar.

### Food Delivery Services

![Food Services](https://res.cloudinary.com/dfjpdzsin/image/upload/foodservices_bhyvvy.png "Food Services Screenshot")
A Higly responsive section created using raw scss.

### Detail Page

![Food Detail](https://res.cloudinary.com/dfjpdzsin/image/upload/fooddetail_y09vxx.png "Food Services Screenshot")
I have used `SerializerMethodField` from the serializer class in rest_framework to group similar products together.

```bash
class ProductSerializer(serializers.ModelSerializer):
  category=CategorySerializer(read_only=True)
  relatedImage=serializers.SerializerMethodField(read_only=True)
  class Meta:
    model=Product
    fields=(
      "id",
      "productName",
      "category",
      "price",
      "description",
      "productImage",
      "relatedImage"
    )
  def get_relatedImage(self,obj):
    item=RelatedProductImage.objects.filter(product_id=obj.pk)
    if item is not None:
      return RelatedProductImageSerializer(item, many=True, context=self.context).data
    return None
```

### Card

![Card Screenshot](https://res.cloudinary.com/dfjpdzsin/image/upload/foodmaincard_psf11v.png "Card Screenshot")

This card is bult with pure scss, `framer-motion` and bootstrap to create beatiful animation when hovering. The UI is higly responsive. I have used `react-tostify` to advance user experience while shopping by creating notification when an item is added into the cart.

### Testimonials

![](https://res.cloudinary.com/dfjpdzsin/image/upload/foodtestimonials_c5zvbl.png)

This beautiful testimonials component is created using `slick-carousel`. It has simple implementation but leaves a long lasting impression to the user. The right image has been generated using AI.

# Installation

## React

### Cloning the site

To clone the project, ensure you have git installed

```bash
git clone https://github.com/DisonUyoga/food_delivery_ecommerce.git
```

```bash
cd food_delivery_ecommerce
```

```bash
npm i
```

```bash
npm run dev
```

## Django Rest

```bash
git clone https://github.com/DisonUyoga/food_backend.git
```

```bash
cd food_backend
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
