# Paradise Nursery | e-plantShopping

Welcome to the **Paradise Nursery** Shopping Application! This project is a React-based single-page application (SPA) that allows users to browse categorized house plants, add them to a global shopping cart, and manage their orders dynamically.

## 🚀 Live Demo

### **[Click Here to Visit the Live Application](PASTE_YOUR_DEPLOYED_GITHUB_PAGES_LINK_HERE)**

_(If the link doesn't open, please copy and paste the URL into your browser)_

---

## 📖 Project Overview

This project was developed as a final assessment to demonstrate proficiency in **React** and **Redux**. It focuses on managing global application state, handling user events, and performing dynamic DOM updates based on the shopping cart status.

## ✨ Key Features

### 1. Landing Page (`AboutUs.jsx`)

- Visually appealing background image with company branding.
- A "Get Started" button that seamlessly navigates users to the shopping area.
- Description of the company mission.

### 2. Product Listing Page (`ProductList.jsx`)

- Displays a variety of plants organized by categories (e.g., Air Purifying, Aromatic, Low Maintenance).
- **Smart "Add to Cart" Buttons:**
  - Adds the item to the Redux store.
  - Instantly updates the Navbar cart counter.
  - **Visual Feedback:** The button becomes disabled and changes text to "Added to Cart" to prevent duplicate additions of the same unique item type.

### 3. Shopping Cart (`CartItem.jsx`)

- **Global State Management:** Uses `CartSlice.jsx` to track items.
- **Dynamic Calculations:**
  - Automatically calculates the **Total Cart Amount**.
  - Calculates the **Subtotal** for each item row.
- **Interactivity:**
  - **Increment (+):** Increases quantity.
  - **Decrement (-):** Decreases quantity (removes item if quantity reaches 0).
  - **Delete:** Instantly removes the item from the cart.
  - **Navigation:** "Continue Shopping" button returns the user to the product list with the state preserved.

### 4. Navigation Bar (`Navbar.jsx`)

- Persistent navigation across views.
- **Dynamic Badge:** A red badge on the cart icon updates in real-time to show the total number of items in the cart.

---

## 🛠️ Technologies Used

- **React.js** (Functional Components, Hooks: `useState`, `useEffect`)
- **Redux Toolkit** (`createSlice`, `configureStore`)
- **React-Redux** (`Provider`, `useSelector`, `useDispatch`)
- **Vite** (Build tool)
- **CSS** (Responsive styling)

---

## 💻 How to Run Locally

If you wish to run this project on your local machine:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/peterSoroush/e-plantShopping.git](https://github.com/peterSoroush/e-plantShopping.git)
   Navigate to the project folder:
   ```

Bash

cd e-plantShopping
Install dependencies:

Bash

npm install
Start the application:

Bash

npm run dev
Then open the localhost link provided in the terminal (usually http://localhost:5173).

📂 Project Structure
src/CartSlice.jsx: Contains the Redux logic (reducers) for addItem, removeItem, and updateQuantity.

src/store.js: Configures the global Redux store.

src/ProductList.jsx: Main shopping page logic.

src/CartItem.jsx: Cart management and total cost logic.

Author: Peter Soroush
