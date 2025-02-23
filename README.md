# Simple Cart Context

This is a simple cart web application built using React. It demonstrates the use of the `useContext` hook for state management.

## Features

-  Add items to the cart
-  Remove items from the cart
-  View the total price of items in the cart

## Technologies Used

-  React
-  useContext hook for state management

## Getting Started

Follow these instructions to set up and run the project on your local machine.

### Prerequisites

-  Node.js
-  npm (Node Package Manager)

### Installation

1. Clone the repository:
   ```bash
   git clone /path/to/your/repository.git
   ```
2. Navigate to the project directory:
   ```bash
   cd simple-cart
   ```
3. Install the dependencies:
   ```bash
   npm install
   ```

### Running the App

1. Start the development server:
   ```bash
   npm run dev
   ```
2. Open your browser and navigate to `http://localhost:5173` to see the app in action.

## Usage

-  To add an item to the cart, click the "Add to Cart" button next to the item.
-  To remove an item from the cart, click the "Remove" button next to the item in the cart.
-  The total price of the items in the cart will be displayed at the bottom of the cart.

## State Management with useContext

This app uses the `useContext` hook to manage the state of the cart. The `CartContext` provides the cart state and dispatch functions to add and remove items from the cart.

```javascript
// ...existing code...
import React, { createContext, useReducer, useContext } from "react";

// Create a context for the cart
const CartContext = createContext();

// ...existing code...

// Custom hook to use the CartContext
const useCart = () => {
   return useContext(CartContext);
};

// ...existing code...
```

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.
