# MiniKart - Premium Fashion & Lifestyle E-Commerce Marketplace

MiniKart is a production-ready full-stack fashion e-commerce platform inspired by the shopping experience of top marketplace applications like Myntra, styled with a warm **Sandal Cream (`#F7E8D5`)**, **Primary Orange (`#FF7A00`)**, and **Brown (`#5A3825`)** color palette.

---

## Key Features

### Customer Storefront
- **Sticky Navigation Header**: Brown MiniKart typography logo, real-time search bar autocomplete, categories nav, wishlist badge, cart badge, user profile menu.
- **Hero Banner Section**: Promotional banner with curved abstract shapes, orange gradients, offer badge ("UP TO 50% OFF"), and action buttons.
- **Circular Category Edits**: Men, Women, Kids, Beauty, Footwear, Accessories, Home & Living.
- **Product Catalog**: Multi-criteria filters (Category, Price Slider, Brand, Star Rating), Sorting (Price Low-to-High, High-to-Low, Latest, Best Selling), and Pagination.
- **Product Detail Page**: Multiple thumbnail image gallery with zoom preview, size selector, color picker, stock level indicator, quantity picker, add to cart & buy now, customer reviews & write-review form.
- **Shopping Cart**: Item quantity update, coupon code apply/remove with discount calculation, shipping cost & tax breakdown.
- **Checkout & Razorpay Payment**: Shipping address selector / add address modal, order summary, Razorpay payment modal supporting UPI, Cards, Net Banking, Mobile Wallets & COD.
- **Order Success Celebration**: Festive confetti celebration, printable PDF invoice download, estimated delivery tracking status bar.
- **User Dashboard**: Profile details editor, order history with tracking timeline, saved addresses, available discount coupons.

### Enterprise Admin Panel (`/admin`)
- **Admin Login**: Preset credentials (`admin@minikart.com` / `admin123`).
- **Admin Dashboard**: Key metrics (Total Revenue, Total Orders, Total Customers, Total Products, Today's Sales, Monthly Sales, Pending, Delivered), Revenue by Category charts, Recent sales trends.
- **Product Management**: Add, edit, delete products, manage stock levels, sizes, colors, and multiple image URLs.
- **Category Management**: Category CRUD.
- **Order Management**: Order listing with status filter, quick status updater dropdown (Pending -> Processing -> Shipped -> Out For Delivery -> Delivered -> Cancelled), invoice generation.
- **Customer Management**: Customer search, total spend & order count metrics, block/unblock customer toggle.
- **Inventory Management**: Stock level status, Low stock alerts (&le; 10), Out of stock list, restock control.
- **Coupon Management**: Create, edit, toggle coupons (Code, discount %, min order amount, expiry, usage limits).
- **Banner Management**: Add, edit, delete hero banners and promo cards.
- **Review Moderation**: Moderate customer reviews.
- **Return Management**: Process return requests & refund status.
- **Analytics Dashboard**: Export PDF and CSV reports.

---

## Tech Stack

- **Frontend**: React.js, Vite, Bootstrap 5, React Router 6, Axios, Lucide Icons, Canvas Confetti, jsPDF.
- **Backend**: Node.js, Express.js, JWT, bcryptjs, Razorpay SDK, Mongoose.
- **Database**: MongoDB (Supports MongoDB Atlas with automatic fallback to `mongodb-memory-server` for out-of-the-box local execution).

---

## Running Locally

### 1. Start Backend Server
```bash
cd backend
npm install
npm start
```
*The backend server will run on `http://localhost:5000`.*

### 2. Start Frontend App
```bash
cd frontend
npm install
npm run dev
```
*The frontend Vite dev server will run on `http://localhost:3000`.*

---

## Preset Login Credentials

- **Admin Login**: `admin@minikart.com` / `admin123`
- **Customer Login**: `user@minikart.com` / `user123`
