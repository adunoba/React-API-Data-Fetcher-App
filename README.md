# React API Data Fetcher App
A React application designed to fetch data from a public API and display it in a structured list. This project emphasizes best practices in component reusability and separation of concerns by utilizing a dedicated list component.

Features
Data Fetching: Fetches data from the JSONPlaceholder API (/posts endpoint).

Loading Indicator: Displays a clear loading animation while data is being fetched.

Error Handling: Provides user-friendly error messages if the API request fails.

Reusable Component: Utilizes a separate ItemList component to render the fetched data, promoting modularity and reusability.

Responsive Design: The layout is responsive and adapts well to various screen sizes.

Modern Styling: Styled with Tailwind CSS for a clean, modern, and engaging user interface.

Technologies Used
React: A JavaScript library for building user interfaces, leveraging useState for state management and useEffect for side effects (data fetching).

Tailwind CSS: A utility-first CSS framework used for rapid UI development and responsive design.

How to Run Locally
To get this application up and running on your local machine, follow these steps:

Prerequisites: Ensure you have Node.js and npm (or yarn) installed on your system.

Create a React Project (if you don't have one):
If you don't have an existing React project, you can create one using Create React App:

npx create-react-app my-api-fetcher-app
cd my-api-fetcher-app

Install Tailwind CSS:
Navigate into your project directory and install Tailwind CSS:

npm install -D tailwindcss
npx tailwindcss init

Configure Tailwind CSS:
Update your tailwind.config.js file to include paths to all of your component files so Tailwind can scan them for classes:

// tailwind.config.js
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

Add the Tailwind directives to your main CSS file (e.g., src/index.css):

/* src/index.css */
@tailwind base;
@tailwind components;
@tailwind utilities;

Place the Code:
Replace the content of your src/App.js file with the provided React code for the App and ItemList components.

Start the Development Server:
Run the following command in your project's root directory:

npm start

This will compile the application and open it in your default web browser, typically at http://localhost:3000.

Usage
Upon launching the application, it will automatically fetch data from the JSONPlaceholder API. You will see a loading message, and once the data is retrieved, a list of post titles and bodies will be displayed.
