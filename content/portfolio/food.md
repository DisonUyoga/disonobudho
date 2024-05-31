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
