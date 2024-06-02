---
title: "Amazing React 19 New Features !!!"
date: 2024-05-30T12:14:34+06:00
description: "Major changes in React"
author: "Dison Obudho"
type: "post"
---

Example: Fetching Data with `use`
To demonstrate the use hook, let's create a simple example that fetches data from an API.

1. Create a data fetching function:

```bash
const fetchData = async () => {
  const response = await fetch('https://jsonplaceholder.typicode.com/posts');
  const data = await response.json();
  return data;
};

```

2. Use the use hook in your component:

```bash
import React, { use } from 'react';

const DataFetchingComponent = () => {
  const data = use(fetchData());

  return (
    <div>
      <h1>Fetched Data</h1>
      <ul>
        {data.map((item) => (
          <li key={item.id}>{item.title}</li>
        ))}
      </ul>
    </div>
  );
};

export default DataFetchingComponent;

```

Key Points:

1. Automatic Suspense Handling:

The use hook automatically suspends rendering until the promise passed to it resolves.
This means you don’t need to manually manage loading states; React handles it for you.

2. Server Components:

The use hook is particularly powerful in server components where data fetching can be done on the server before the HTML is sent to the client.

3. Error Handling:

If the promise rejects, the use hook will propagate the error, and you can handle it using React's error boundaries.

Complete Example with Error Handling:

1. Create an error boundary component:

```bash
import React from 'react';

class ErrorBoundary extends React.Component {
  constructor(props) {
    super(props);
    this.state = { hasError: false };
  }

  static getDerivedStateFromError(error) {
    return { hasError: true };
  }

  componentDidCatch(error, info) {
    console.error("Error occurred:", error, info);
  }

  render() {
    if (this.state.hasError) {
      return <h1>Something went wrong.</h1>;
    }
    return this.props.children;
  }
}

export default ErrorBoundary;

```

2. Use the use hook with the error boundary:

```bash
import React, { use } from 'react';
import ErrorBoundary from './ErrorBoundary';

const fetchData = async () => {
  const response = await fetch('https://jsonplaceholder.typicode.com/posts');
  if (!response.ok) {
    throw new Error('Network response was not ok');
  }
  const data = await response.json();
  return data;
};

const DataFetchingComponent = () => {
  const data = use(fetchData());

  return (
    <div>
      <h1>Fetched Data</h1>
      <ul>
        {data.map((item) => (
          <li key={item.id}>{item.title}</li>
        ))}
      </ul>
    </div>
  );
};

const App = () => (
  <ErrorBoundary>
    <DataFetchingComponent />
  </ErrorBoundary>
);

export default App;

```

In this complete example, we’ve added an error boundary to catch any errors that occur during data fetching and display a fallback UI. The use hook simplifies asynchronous data handling, making your components cleaner and more concise

Summary:

- The use hook allows you to work with promises more naturally.
- It suspends rendering until the promise resolves.
- It integrates well with server components.
- You can handle errors using React's error boundaries.
