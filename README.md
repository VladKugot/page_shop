# 📱 React Product Catalog

This project is a **Product Catalog** implemented with **React** and **TypeScript**, featuring a shopping cart, favorites, filtering, sorting, pagination, category pages, and detailed product pages. The design follows specified UI kits with light and dark themes and uses modern frontend best practices.

---

## 🔗 Live Demo  
[DEMO LINK](https://vladkugot.github.io/react_phone-catalog/)

## 🎨 Design Reference  
[DESIGN LINK Light](https://www.figma.com/design/7JTa0q8n3dTSAyMNaA0u8o/Phone-catalog--V2--Rounded-Style-3?node-id=0-1)

[DESIGN LINK Dark](https://www.figma.com/design/BUusqCIMAWALqfBahnyIiH/Phone-catalog--V2--Original-Dark?node-id=0-1&p=f)

---

## ⚙️ Technologies Used

- React + TypeScript  
- React Router for navigation  
- SCSS Modules for styling  
- Context API or Redux for state management (cart and favorites)  
- ESLint + Prettier + Husky for code quality and Git hooks  
- LocalStorage for persistent cart and favorites data  

---

## 📦 Project Features

- **Sticky header** with logo, navigation, favorites, and cart icons  
- Responsive footer with GitHub repo link and smooth Back-to-Top button  
- Visually hidden `<h1>` on home page for accessibility  
- **Home page** with:
  - Pictures slider (auto and manual navigation)
  - Hot prices product slider (products with biggest discounts)
  - Shop by category block linking to `/phones`, `/tablets`, `/accessories`
  - Brand new products slider sorted by year  
- **Category pages** (`/phones`, `/tablets`, `/accessories`):
  - Loads relevant products by category
  - Displays products list with loading and error states
  - Sort products by newest, alphabetical, or cheapest (via URL param `?sort=...`)
  - Pagination with configurable items per page and URL syncing
  - Search functionality with debounced input and query syncing via `?query=...`  
- **Product details page** (`/product/:productId`):
  - Loader while fetching product data
  - Displays product details, selectable colors and capacities as radio inputs
  - "You may also like" block with suggested products
  - Back button (browser-like navigation)
  - Breadcrumb navigation
  - "Product not found" message for invalid IDs  
- **Shopping cart page** (`/cart`):
  - List of cart items with quantity controls (+/-), remove button, and total calculation
  - "Add to cart" button disabled if already in cart, shows "Added to cart"
  - Cart saved and loaded from `localStorage`
  - Checkout modal dialog with confirmation and cart clearing  
- **Favorites page** (`/favorites`):
  - List of favorite products with add/remove heart button
  - Favorites count in header icon
  - Favorites saved and loaded from `localStorage`  
- **NotFoundPage** for all unknown routes with link back to home  
- Smooth hover effects and image scaling on hover  
- Optional features:  
  - Color theme switching (light/dark)  
  - Skeleton loaders for better UX  
  - Language switching support  

---

## 🚀 How to Run the Project Locally

### Prerequisites

- Node.js (>=14 recommended)  
- npm or yarn package manager  

### Setup Steps

1. **Clone the repository** (or your fork):
   ```bash
   git clone https://github.com/<your_account>/react-product-catalog.git
   cd react-product-catalog

2. **Install Dependencies**
```bash
npm install
```

3. **Start the Development Server**
```bash
npm start
```
