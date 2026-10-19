# Paradise Nursery Shopping Application

A responsive e-commerce web application for **Paradise Nursery**, an online plant store where customers can browse, select, and purchase various houseplants.

Developed as the Final Capstone Project for the **"Developing Front-End Apps with React"** course offered by IBM on Coursera.

---

## 🌿 Project Overview

Paradise Nursery is designed to bring nature closer to plant enthusiasts. The application provides an intuitive and seamless shopping experience, allowing users to:
- Learn about Paradise Nursery and its mission on an interactive landing page.
- Browse a rich catalog of categorized houseplants (Air Purifying, Aromatic & Fragrant, Insect Repellent, Medicinal, and Low Maintenance).
- View plant details including high-resolution thumbnails, names, descriptions, and unit prices.
- Add plants to a centralized shopping cart powered by **Redux Toolkit**.
- Adjust item quantities dynamically (increment/decrement) or remove items from the cart.
- View subtotal costs for each plant item and the overall total cart value calculated in real time.

---

## ✨ Features

1. **Interactive Landing Page (`App.jsx`, `AboutUs.jsx`, `App.css`)**:
   - Company branding with the slogan *"Where Green Meets Serenity"*.
   - Immersive greenhouse background image.
   - Comprehensive "About Us" section highlighting our mission and expert plant care standards.
   - Smooth animated transition to the plant catalog via the "Get Started" button.

2. **Categorized Product Listing (`ProductList.jsx`, `ProductList.css`)**:
   - Organized into 5 distinct categories with 6 unique plants per category (30 plants total).
   - "Add to Cart" button that dynamically disables itself once added and indicates "Added to Cart".
   - Sticky navigation bar with quick links to **Home**, **Plants**, and **Cart**.
   - Dynamic cart icon showing the total number of items in real time.

3. **State Management (`CartSlice.jsx`, `store.js`)**:
   - Redux Toolkit slice managing cart state.
   - Actions: `addItem`, `removeItem`, and `updateQuantity`.

4. **Shopping Cart View (`CartItem.jsx`, `CartItem.css`)**:
   - Displays all selected plants with thumbnail images, names, and unit prices.
   - Quantity controls (`+` and `-`) to increment or decrement counts. Decreasing to zero automatically removes the item.
   - Subtotal calculations for each plant and grand total calculation for the whole cart.
   - "Delete" button for removing any item instantly.
   - "Continue Shopping" button returning users directly to the product catalog.
   - "Checkout" button displaying a "Coming Soon" notification.

---

## 🛠️ Technology Stack

- **Frontend Framework**: [React 18](https://react.dev/)
- **State Management**: [Redux Toolkit](https://redux-toolkit.js.org/) & [React-Redux](https://react-redux.js.org/)
- **Build Tool & Bundler**: [Vite](https://vitejs.dev/)
- **Styling**: Vanilla CSS3 (Flexbox, responsive media queries, CSS transitions)

---

## 📂 Project Structure

```text
├── public/                 # Static assets
├── src/
│   ├── assets/             # Images and media
│   ├── AboutUs.css         # Styling for About Us section
│   ├── AboutUs.jsx         # Company background and mission component
│   ├── App.css             # Landing page and global styling
│   ├── App.jsx             # Main application container & landing page
│   ├── CartItem.css        # Shopping cart page styling
│   ├── CartItem.jsx        # Shopping cart view and item management
│   ├── CartSlice.jsx       # Redux Toolkit slice for shopping cart
│   ├── ProductList.css     # Product listing and navbar styling
│   ├── ProductList.jsx     # Plant catalog grouped by category
│   ├── index.css           # Global typography and base styles
│   ├── main.jsx            # Application entry point with Redux Provider
│   └── store.js            # Redux store configuration
├── index.html              # HTML entry template
├── package.json            # Project dependencies and npm scripts
├── vite.config.js          # Vite configuration
└── README.md               # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) (v16 or higher) and `npm` installed.

### Installation

1. Clone this repository or download the project files:
   ```bash
   git clone <YOUR_REPOSITORY_URL>
   cd "Developing Front-End Apps with React"
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

### Running the App Locally

To start the Vite development server:
```bash
npm run dev
```

Open your browser and navigate to `http://localhost:5173` (or the URL displayed in your terminal).

### Building for Production

To create an optimized production build:
```bash
npm run build
```

---

## 📝 Grading Criteria Mapping

| Task | File | Description |
|---|---|---|
| Task 1 | `README.md` | Contains project name and full application details. |
| Task 2 | `src/AboutUs.jsx` | Details about Paradise Nursery, company mission, and values. |
| Task 3 | `src/App.css` | Implements background image and styling for the landing page. |
| Task 4 | `src/App.jsx` | Landing page with company name, tagline, and "Get Started" button. |
| Task 5 | `src/CartSlice.jsx` | Redux slice managing cart items, add, remove, and update actions. |
| Task 6 | `src/ProductList.jsx` | Plant catalog (6 plants x 5 categories), add-to-cart, navbar, and cart badge. |
| Task 7 | `src/CartItem.jsx` | Cart page with subtotals, grand total, quantity update, delete, and navigation. |

---

## 📄 License

This project is licensed under the MIT License.