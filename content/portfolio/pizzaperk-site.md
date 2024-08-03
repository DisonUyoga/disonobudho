+++
categories = ["web-dev"]
coders = ["DisonObudho"]
date = 2024-06-19T23:00:00Z
description = "PizzaPerk Food Delivery Site (production ready)"
github = ["https://github.com/DisonUyoga/pizza-perk.git"]
image = "https://cdn.svgporn.com/logos/nextjs.svg"
title = "FullStack Responsive Food Delivery Site"
type = "post"
[[tech]]
logo = "https://cdn.svgporn.com/logos/nextjs.svg"
name = "PizzaPerk"
url = "https://pizza-perk.vercel.app/"


+++

---

## Site Url:

[PizzaPerk Site](https://pizza-perk.vercel.app/)

### Project Overview: PizzaPerk Food Delivery Site

**Project Name:** PizzaPerk

**Tech Stack:**

- **Frontend:** Next.js (using SSR, parallel routes, intercepted routes), Redux for state management, TypeScript for type safety and error-free code.
- **Backend:** Supabase for database management and backend services.
- **Testing:**
  - **end-to-end and component testing**(cypress)
  - **unit testing**(jest and react testing library)

---

### Features and Functionality

#### 1. **Server-Side Rendering (SSR)**

- **Objective:** Improve SEO and provide a faster initial load.
- **Implementation:** Key pages, such as the homepage, menu, and order details, are rendered on the server. This allows the site to deliver content-rich pages quickly and enhance the user experience.

watch video`
[![Video Thumbnail](https://res.cloudinary.com/dfjpdzsin/image/upload/v1722703891/modalplaceholder_rhjmrg.jpg)](https://res.cloudinary.com/dfjpdzsin/video/upload/v1722704239/pizzasitessrexplanation_amtfgg.mp4)

#### 2. **Parallel Routes**

- **Objective:** Improve load times and enhance user experience by loading multiple routes simultaneously.
- **Implementation:** Used Next.js's ability to load components in parallel, particularly for complex pages like the menu with multiple categories etc.

#### 3. **Intercepted Routes**

- **Objective:** Provide a smoother navigation experience by intercepting routes and handling them appropriately without a full page reload.
- **Implementation:** This feature is particularly useful for modals and sidebars. For example, clicking on a pizza item opens a modal with the item details without navigating away from the current page.

#### 4. **Redux for State Management**

- **Objective:** Maintain a predictable state across the application.
- **Implementation:** Used Redux to manage the application state, particularly for user authentication, cart management, order tracking, and user preferences. Actions and reducers are defined to handle the state transitions in a predictable manner.

#### 5. **Supabase Backend**

- **Objective:** Provide a robust backend service with real-time capabilities.
- **Implementation:** Supabase is used for database management, user authentication, and real-time data synchronization. It provides an API that the frontend interacts with to perform CRUD operations, manage user sessions, and handle real-time updates (e.g., order status changes).

#### 6. **TypeScript**

- **Objective:** Ensure type safety and reduce runtime errors by catching issues at compile time.
- **Implementation:** TypeScript is used extensively throughout the project to define types for components, props, state, and API responses. This practice helps in maintaining clean, readable, and error-free code.

---

### Key Pages and Components

#### **Homepage**

- **Features:** Display featured pizzas and special deals.
- **SSR Implementation:** Pre-render the page on the server to deliver content quickly.

#### **Menu Page**

- **Features:** Display categories of pizzas.
- **Parallel Routes:** Load multiple categories and filters simultaneously to enhance performance.

#### **Pizza Detail Modal**

- **Features:** Show detailed information about a pizza item, including price, and customization options.
- **Intercepted Routes:** Open as a modal from the menu page without a full page reload.

#### **Cart**

- **Cart Logic**: Users can access their cart from any screen, with real-time updates reflecting item additions and modifications. Interactive modals guide users through selecting pizza sizes, drink options, and customizing their orders, ensuring a smooth and efficient ordering process.

- Implemented a dynamic cart system where the total adjusts effectively when items are added or removed.

  - Price tags automatically update based on pizza sizes, ensuring accurate pricing.
  - Developed a logic to distinguish between drinks (no size update) and pizzas (size update required), ensuring clear categorization.

#### **User Profile**

- **Features:** Display user information, order history, and settings.
- **Parallel Routes:** Load different sections (orders, settings) in parallel for a smoother experience.

---

### Project Structure

**Frontend Directory:**

- **/pages:** Contains all the page components, leveraging Next.js's file-based routing.
- **/components:** Reusable UI components like buttons, modals, and forms.
- **/store:** Redux store configuration, actions, and reducers.
- **/utils:** Utility functions and hooks.
- **/types:** TypeScript type definitions.

**Backend Directory:**

- **/supabase:** Configuration and API integration with Supabase.
- **/services:** Backend services and functions interacting with Supabase.

---

### Summary

PizzaPerk leverages the power of Next.js for an optimized user experience through server-side rendering, parallel and intercepted routes, and robust state management with Redux. The use of TypeScript ensures type safety and reduces errors during development. Supabase provides a powerful backend solution, enabling real-time updates and efficient data management. This combination of technologies ensures PizzaPerk is fast, reliable, and user-friendly.

The following react depencies were used in this project:

      "@chakra-ui/icons": "^2.1.1",
    "@chakra-ui/react": "^2.8.2",
    "@clerk/nextjs": "^5.2.6",
    "@emotion/react": "^11.13.0",
    "@emotion/styled": "^11.13.0",
    "@fortawesome/fontawesome-svg-core": "^6.6.0",
    "@fortawesome/free-solid-svg-icons": "^6.6.0",
    "@fortawesome/react-fontawesome": "^0.2.2",
    "@reduxjs/toolkit": "^2.2.6",
    "@stripe/react-stripe-js": "^2.7.3",
    "@stripe/stripe-js": "^4.1.0",
    "@supabase/auth-helpers-nextjs": "^0.10.0",
    "@supabase/ssr": "^0.4.0",
    "@supabase/supabase-js": "^2.44.4",
    "@tanstack/react-query": "^5.51.15",
    "aos": "^2.3.4",
    "axios": "^1.7.2",
    "clsx": "^2.1.1",
    "firebase": "^10.12.4",
    "framer-motion": "^11.3.18",
    "install": "^0.13.0",
    "loadash": "^1.0.0",
    "lodash": "^4.17.21",
    "lorem-ipsum": "^2.0.8",
    "next": "14.2.5",
    "npm": "^10.8.2",
    "react": "^18",
    "react-countdown": "^2.3.5",
    "react-dom": "^18",
    "react-error-boundary": "^4.0.13",
    "react-hot-toast": "^2.4.1",
    "react-icons": "^5.2.1",
    "react-merge-refs": "^2.1.1",
    "react-redux": "^9.1.2",
    "react-slick": "^0.30.2",
    "slick-carousel": "^1.8.1",
    "svix": "^1.25.0"

### Launching the PizzaPerk Food Delivery Site

My PizzaPerk food delivery site, built with Next.js, is designed to offer an optimized, seamless user experience. Here’s how it launches:

1. **Server-Side Rendering (SSR)**: We use SSR to pre-render the homepage, ensuring fast load times and improved SEO. This means that key content is ready to go as soon as the user lands on the site.

2. **React Suspense for Loading States**: To handle data fetching gracefully, we leverage React's Suspense. This allows us to show a loading indicator while waiting for data to be loaded, providing users with immediate feedback that the content is being retrieved.

3. **Chakra UI Spinner**: The loading indicator is implemented using Chakra UI's Spinner component. When the homepage is fetching data, the Chakra Spinner is displayed, centered on the screen, ensuring a visually appealing and consistent user experience.

This combination of Next.js for SSR, React Suspense, and Chakra UI for loading states ensures that PizzaPerk delivers a fast, responsive, and user-friendly experience from the moment users visit our site.

`watch video`

[![Video Thumbnail](https://res.cloudinary.com/dfjpdzsin/image/upload/v1722702576/homepahepizzasiteplaceholder_piwwkt.jpg)](https://res.cloudinary.com/dfjpdzsin/video/upload/v1722701865/homepagepizzaperksite_a0ei5e.mp4)

---

### Product Detail Modal Implementation in PizaPerk Food Delivery App

**Project:** PizaPerk Food Delivery App  
**Technology Stack:** Next.js, Redux

**Description:**

In the PizaPerk food delivery app, I implemented a versatile product detail modal that can be accessed from any page within the application. The modal dynamically determines whether the selected item is a pizza or a drink and displays the appropriate components accordingly. Here’s a detailed breakdown of the implementation:

1. **Dynamic Display Based on Item Type:**

   - The modal automatically detects the type of item being viewed. If the item is a pizza, the modal displays a size selection component. For drinks, this component is omitted.

2. **Global Access:**

   - The product detail modal is designed to be accessible from any page in the app. This ensures a seamless user experience, allowing users to view product details and make selections without navigating away from their current page.

3. **Implementation Using Next.js and Redux:**
   - **Next.js:** Utilized Next.js for server-side rendering and efficient routing.
   - **Redux:** Managed the state of the modal using Redux to ensure consistent behavior across the application.

**Key Features:**

- **Parallel and Intercepted Routing:**

  - Implemented parallel routing to allow the modal to open over any current route, without disrupting the user’s navigation flow.
  - Intercepted routing ensures that when the modal is closed, the user returns to their previous state seamlessly.

- **Component Structure:**
  - Created a reusable `ProductDetailModal` component.
  - The component checks the item type and conditionally renders the `SizeSelection` component if the item is a pizza.

**Code Snippet:**

```javascript
// ProductDetailModal.js
import { pizzas, sizes } from "@/data";
import { Tables } from "@/database.types";
import {
  addToCart,
  CartItems,
  selectSize,
  setIsPizza,
  setTogglePriceDependingOnSize,
  updateCartTotalAfterSizeChange,
} from "@/features/slices/cartSlice";
import { setProduct } from "@/features/slices/productSlice";
import { useAppDispatch, useAppSelector } from "@/lib/hook";
import { PizzaSize } from "@/type";
import {
  Box,
  Button,
  Center,
  Flex,
  Modal,
  ModalBody,
  ModalCloseButton,
  ModalContent,
  ModalFooter,
  ModalHeader,
  ModalOverlay,
  Text,
  useDisclosure,
} from "@chakra-ui/react";
import { motion } from "framer-motion";
import { useRouter, useSearchParams } from "next/navigation";
import { useEffect, useState } from "react";
import { createPortal } from "react-dom";
import toast from "react-hot-toast";
import PriceCard from "./PriceCard";
import ProductImage from "./ProductImage";
import SelectSize from "./SelectSize";

const ProductDetailModal = () => {
  const dispatch = useDispatch();
  const { item, isOpen } = useSelector((state) => state.modal);

  if (!isOpen) return null;

  return createPortal(
    <Modal isOpen={isOpen} onClose={onClose}>
      <ModalOverlay />
      <ModalContent>
        <ModalHeader>{product.name}</ModalHeader>
        <ModalCloseButton onClick={() => router.back()} />
        <ModalBody>
          {product && (
            <Center>
              {pizzas[0].img && product.image && (
                <Box
                  position={"relative"}
                  width={["100vw", "50vw"]}
                  h={"50vh"}
                  data-aos="fade-down"
                  data-aos-easing="linear"
                  data-aos-duration="1500"
                >
                  <ProductImage fallback={pizzas[0].img} path={product.image} />
                </Box>
              )}
            </Center>
          )}
          <PriceCard product={product} />
          <Text
            fontSize={"10px"}
            fontWeight={600}
            mt={2}
            color={"#050152"}
            data-aos="zoom-in"
            data-aos-duration="1500"
          >
            The offer only applies to Extra Large
          </Text>
          {determineIfItemIsPizza && (
            <Flex
              flex={1}
              mt={4}
              alignContent={"center"}
              justify={"space-between"}
            >
              {sizes.map((s, index) => (
                <SelectSize
                  key={index}
                  sizes={s}
                  selected={selected}
                  handleSelected={handleSelected}
                  product={product}
                />
              ))}
            </Flex>
          )}

          {product.description && (
            <Text
              mt={10}
              fontSize={["xs", "md"]}
              data-aos="zoom-in"
              data-aos-duration="1500"
            >
              {product.description}
            </Text>
          )}
        </ModalBody>

        <ModalFooter>
          <MotionButton
            whileHover={{ scale: 1.1 }}
            whileTap={{ scale: 0.9 }}
            transition={{ type: "spring", stiffness: 300 }}
            size={["sm", "md"]}
            fontSize={["xs", "md"]}
            colorScheme="blue"
            mr={3}
            onClick={() => {
              router.back();
              onClose();
            }}
          >
            Back
          </MotionButton>
          <MotionButton
            whileHover={{ scale: 1.1 }}
            whileTap={{ scale: 0.9 }}
            transition={{ type: "spring", stiffness: 300 }}
            size={["sm", "md"]}
            fontSize={["xs", "md"]}
            colorScheme="blue"
            bg={"#088d25"}
            mr={3}
            onClick={() => addProductToCart(product)}
          >
            Add to Cart
          </MotionButton>
        </ModalFooter>
      </ModalContent>
    </Modal>,
    document.getElementById("modal-root")!
  );
};

export default ProductDetailModal;
```

**State Management:**

```javascript
// actions.js
 const [loading, setLoading] = useState(false);
  const [selectionLoader, setSelectionLoader] = useState(false);
  const searcParams = useSearchParams();

  const dispatch = useAppDispatch();
  const router = useRouter();
  const {
    totalAmount,
    totalQuantity,
    sizes: selected,
  } = useAppSelector((state) => state.cart);

  const cartItems = useAppSelector((state) => state.cart.cartItems);
  const searchParams = useSearchParams();
  const [cartProduct, setCartProduct] = useState<CartItems | undefined>();
  const [openZoom, setOpenZoom] = useState(false);
  const [priceSize, setPriceSize] = useState<number | null>(null);

  const { isOpen, onOpen, onClose } = useDisclosure();
  const determineIfItemIsPizza = !!(
    product?.size_large ||
    product?.size_medium ||
    product?.size_small
  );
  const update = searchParams.get("update");
  useEffect(() => {
    OpenModal();
  }, []);
  useEffect(() => {
    if (determineIfItemIsPizza) {
      dispatch(setIsPizza({ isPizza: determineIfItemIsPizza }));
    }
    if (cartItems) {
      checkIfItemIsAlreadyInTheCart(cartItems);
    }
    if (cartItems && cartProduct) {
      changeCartTotalWhenSizeIsChanged(cartItems);
    }
  }, [cartItems]);
  useEffect(() => {
    dispatch(setTogglePriceDependingOnSize({ price: product.price }));
    dispatch(
      selectSize({
        size: "XL",
        product,
      })
    );
    if (product) {
      dispatch(setProduct({ product }));
    }
  }, [product, determineIfItemIsPizza]);

  function OpenModal() {
    onOpen();
  }

  const handleSelected = (size: PizzaSize | null | undefined) => {
    size != null
      ? toast.success(
          `You have selected ${
            size == "S"
              ? "small"
              : size === "M"
              ? "medium"
              : size === "L"
              ? "large"
              : size === "XL"
              ? "extra large"
              : null
          }`
        )
      : null;
    setSelectionLoader(true);

    try {
      if (!product) return;

      dispatch(
        selectSize({
          size: size as PizzaSize,
          product,
        })
      );

      updateSize();
      if (!size) return;

      togglePriceDependingOnTheSize(product, size);
    } catch (error) {
    } finally {
      setSelectionLoader(false);
    }
  };
  function checkIfItemIsAlreadyInTheCart(c: CartItems[]) {
    const cartItem = cartItems.find((p) => p.id === product?.id) as CartItems;

    if (!cartItem || !product) return;

    setCartProduct(cartItem);
  }

  function togglePriceDependingOnTheSize(
    product: Tables<"products">,
    selectedSize: PizzaSize
  ) {
    switch (selectedSize) {
      case "S":
        dispatch(setTogglePriceDependingOnSize({ price: product.size_small }));

        break;
      case "M":
        dispatch(setTogglePriceDependingOnSize({ price: product.size_medium }));

        break;
      case "L":
        dispatch(setTogglePriceDependingOnSize({ price: product.size_large }));

        break;
      default:
        dispatch(setTogglePriceDependingOnSize({ price: product.price }));
    }
  }
  function changeCartTotalWhenSizeIsChanged(c: CartItems[]) {
    setSelectionLoader(true);
    const item = c.find((p) => p.id === product?.id);

    if (!item) return;

    if (item?.price) {
      dispatch(
        updateCartTotalAfterSizeChange({
          product: item,
          currentPrice: item.price,
        })
      );
    }
    setSelectionLoader(false);
  }
  function updateSize() {
    if (update && cartItems && cartProduct) {
      changeCartTotalWhenSizeIsChanged(cartItems);
      toast.success("item updated");
      router.back();
    }
  }
  function addProductToCart(product: Tables<"products">) {
    dispatch(setIsPizza({ isPizza: determineIfItemIsPizza }));
    if (!product) return;

    try {
      setLoading(true);
      dispatch(
        addToCart({
          product,
          size: selected,
        })
      );
      setLoading(false);
      toast.success("item added to cart");

      router.back();
    } catch (error: any) {
    } finally {
      setLoading(false);
    }
  }
```

This implementation not only enhances the user experience by providing dynamic content but also maintains the state and navigational context, ensuring a smooth and intuitive interaction for users.

`watch video`
[![Video Thumbnail](https://res.cloudinary.com/dfjpdzsin/image/upload/v1722703891/modalplaceholder_rhjmrg.jpg)](https://res.cloudinary.com/dfjpdzsin/video/upload/v1722703883/modalpizzaperksite_p14hux.mp4)

---
