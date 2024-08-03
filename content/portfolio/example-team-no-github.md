+++
categories = ["web-dev"]
coders = ["disonobudho"]
date = 2024-05-15T23:00:00Z
description = "Frontend Developer Assessment Project"
image = "https://cdn.svgporn.com/logos/react.svg"
title = "Near Earth Object Web Service (NEOWS) Website"
type = "post"
[[tech]]
logo = "https://cdn.svgporn.com/logos/react.svg"
name = "Nextjs"
url = "https://gohugo.io/"
+++

---

**Project Description: Near Earth Object Web Service (NEOWS) Website**

I developed a responsive web application for the Near Earth Object Web Service (NEOWS) using a robust stack of modern web technologies. The project involved the following key aspects:

- **Frontend Development:**

  - **React**: Utilized React to build a dynamic and interactive user interface.
  - **TypeScript**: Implemented TypeScript to enhance code quality and maintainability with strong typing and error checking.
  - **Chakra UI**: Employed Chakra UI for a consistent and accessible design system, ensuring a polished and user-friendly experience.
  - **Emotion/React**: Used Emotion for efficient and scalable CSS-in-JS styling, providing a flexible approach to component-level styling.

- **Data Management and Visualization:**

  - **TanStack/React-Table**: Leveraged TanStack/React-Table for powerful and customizable table functionalities, including sorting, filtering, and pagination.
  - **Chart.js**: Integrated Chart.js to visualize NEOWS data effectively, presenting complex information in a clear and interactive manner.
  - **TanStack/React-Query**: Applied TanStack/React-Query for efficient data fetching and state management, optimizing the application's performance and user experience.

- **Backend Communication:**

  - **Axios**: Used Axios for seamless and reliable HTTP requests to the NEOWS API, ensuring smooth data retrieval and integration.

This project highlights my ability to build responsive, data-driven web applications using a combination of advanced technologies. It showcases my proficiency in creating visually appealing and functional user interfaces, managing and visualizing data effectively, and integrating frontend and backend components seamlessly.

---

### Pulic Link to the site:

[neowsApI](https://neos-api.vercel.app/)

### Project Description

There were a total of 5 questions involved in this react interview. The time limit for the interview was 8 hours. However, finishing all the questions was not mandatory. [Near Earth Object Web Service(Neows)](https://api.nasa.gov/#asteroids-neows) API was used to generate data for the UI.

The assesment was based on:

- Appearance and UX of your web app
- Maintainability and Quality of your code
- General approach to solve problems
- Use of dependencies other than required ones
- Your own time management and prioritisation

### Required Dependencies were:

✔ node16+
✔ npm8+
✔ react (latest)
✔ typescript (latest)
✔ github
✔ `axios` and `react-query` ( https://react-query.tanstack.com/overview )
✔ all code is written in `.ts` or `.tsx`

### Tasks

1. Create a spreadsheet that shows a list of up to 10 today's most recent near-earth objects.
   Each row represents one asteroid. The list is sorted by time of the close approach. The latest
   close approach is shown first.
   The spreadsheet features the following columns.- Time: Date and time of the close approach- Asteroid name: Name of the asteroid- Potential Hazard: Is it a potentially hazardous asteroid? (yes/no)- Estimated diameter: Maximum estimated diameter of the asteroid in meters rounded- Miss distance: Distance by which asteroid missed earth in kilometers rounded- Velocity: Relative velocity of asteroid in kilometers per hour rounded
   Remember to use react-query to implement the query.
   Refer to the NeoWs API docs!.

2. Let's extend the previously created spreadsheet. We want to be able to select a date range to
   show asteroids of that date range. To allow this, make two pickers for start date and end date.
   Also, make a "today" button that automatically selects today as the date range. By default, show
   today's most recent objects as before.
   Whenever a new date is selected, the new data is fetched automatically.
3. In the previous task, we showed only up to 10 rows. Since now, our table is able to show
   many more rows, its time to introduce pagination. Paginate your spreadsheet to show 10 results
   with pagination.
   Note: Data doesn't have to be re-fetched when changing pages.
4. Add another column to the table which allows a user to write a note to themselves about an
   asteroid. This note is persisted locally on the user's machine. Whenever data is fetched, show
   the note contents automatically. If no note is found for the row, show a blank field.
5. Use react-query to cache the results of each query based on the start and end dates to speed
   up loading when browsing different dates.
6. Based on the data from the spreadsheet, create a bar chart where the x axis shows individual
   asteroids, and the y axis shows their velocity.

### Complete Project Code

[neowsAPI Complete Project](https://github.com/DisonUyoga/neosAPI.git)

### Project Implementation

I used the following libraries in the project:

- chakra-ui/react
- tanstack/react-query
- axios
- emotion/react
- tanstack/react-table

I relied heavily on tanstack/react-table to generate headless UI. I used Typescript to create complex data types that included index signatures.
