# Paradise Nursery Shopping Application

An elegant, mobile-first e-commerce web application for plant enthusiasts, built with React, Redux Toolkit, and Vite. **Paradise Nursery: Where Green Meets Serenity.**

---

## 🌿 Features

- **Landing Page**:
  - Welcoming hero section with background visuals and company mission statement.
  - Informative "About Us" section detailing the nursery's story and standards of plant care.
  - Smooth transition to the product catalog via the "Get Started" button.

- **Product Catalog**:
  - 30 distinct plants organized into 5 categories:
    - *Air Purifying Plants* (Snake Plant, Spider Plant, Peace Lily, etc.)
    - *Aromatic Fragrant Plants* (Lavender, Jasmine, Rosemary, etc.)
    - *Insect Repellent Plants* (Oregano, Marigold, Geraniums, etc.)
    - *Medicinal Plants* (Aloe Vera, Echinacea, Peppermint, etc.)
    - *Low Maintenance Plants* (ZZ Plant, Pothos, Cast Iron Plant, etc.)
  - Plant cards featuring high-quality images, descriptions, pricing, and dynamic "Add to Cart" buttons.
  - Add to Cart buttons update to "Added to Cart" and disable to prevent accidental duplicates.

- **Shopping Cart**:
  - Real-time cart badge counter displayed in the navigation bar showing total quantity of items.
  - Cart overview displaying item thumbnails, plant names, unit prices, quantity modifiers, and subtotal per item.
  - Interactive increment (`+`) and decrement (`-`) quantity controls (automatically removing items when decremented to zero).
  - Delete button to remove specific items immediately.
  - Automatically calculated grand total cart amount.
  - "Continue Shopping" button returning users seamlessly to the plant catalog.
  - "Checkout" button alerting users of upcoming features.

- **State Management**:
  - Global state managed predictably using Redux Toolkit (`CartSlice.jsx`) with actions for `addItem`, `removeItem`, and `updateQuantity`.

---

## 🛠️ Tech Stack

- **React 18** (Functional components and Hooks)
- **Redux Toolkit** (Global state management)
- **Vite** (Next-generation frontend tooling and fast HMR)
- **CSS3** (Responsive, mobile-friendly layouts)

---

## 📂 Project Structure

```text
├── public/
├── src/
│   ├── assets/
│   ├── AboutUs.css
│   ├── AboutUs.jsx          # Nursery background & mission information
│   ├── App.css
│   ├── App.jsx              # Landing page & view transition controller
│   ├── CartItem.css
│   ├── CartItem.jsx         # Shopping cart review, totals, & item controls
│   ├── CartSlice.jsx        # Redux slice with cart reducers
│   ├── index.css
│   ├── main.jsx             # React DOM root and Redux Provider setup
│   ├── ProductList.css
│   ├── ProductList.jsx      # Plant catalog grid, categories, & cart badge
│   └── store.js             # Redux store configuration
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher recommended)
- npm

### Installation
```bash
# Clone the repository
git clone https://github.com/USERNAME/REPO.git

# Navigate into the project directory
cd repository

# Install dependencies
npm install
```

### Running the Development Server
```bash
npm run dev
```

### Building for Production
```bash
npm run build
```