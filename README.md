### 🐾 Kurd Pets – Online Animal Marketplace (Final Year Project)

![Project Screenshots](available in the kurd-pets repository)
## 📁 Project Sections and Screenshots

- [Home Page](/1%20Homepage.md)
- [Cart Section](/8%20cart-panel.md)
- [Checkout Section](/9%20checkout.md)
- [Payment Section](/10%20payment.md)
- [Admin Dashboard](/7%20Admin%20Dashboard.md)
- [Notification](/11%20notification.md)
- [Blogs Page](/3%20Blogs%20page.md)
- [Products Page](/4%20Products%20page.md)
- [Contact Page](/5%20contact-page.md)
- [Registration](/6%20registration.md)



**Kurd Pets** is a full-stack, role-based online animal and pet-related product platform built as my final year graduation project. 
The platform enables customers to browse, filter, pre-order, and purchase pet-related products, while admins and super admins 
can manage content, orders, and tasks via a secure dashboard.

> ⚠️ **Note**: The source code is private for now, but all UI screenshots and architecture have been shared for demonstration purposes.

## 📦 Tech Stack

### 👨‍💻 Frontend
- **React 19**
- **Pure CSS** (no frameworks like Tailwind or Bootstrap)
- **React Router DOM v7**
- **Framer Motion** (for animations)
- **FontAwesome** (icons)
- **Axios**, **React Toasts**, **React Tooltips**, **React Datepicker**
- **JWT Decode**, **Google Libphonenumber**

### 🧠 Backend
- **Node.js + Express**
- **MySQL** (Relational DB)
- **JWT (Cookies)** for secure auth
- **Cloudinary** (Image Uploads)
- **Nodemailer** (Email Notifications)
- **Multer** (File Uploads)
- **Express Validator**, **UUID**
- **Role-based Access Control**
- **Validation on both Client & Server Side**

---

## 🎯 Project Overview

### 🏠 Public Website Pages
- **Main Page**: Navbar, Hero Section, Featured Collections, Blogs, Products, Brands, Footer.
- **Blogs**: Viewable by anyone. Logged-in users can like, save blogs.
- **Products**:
  - Customers can view, filter, and save products to cart panel.
  - If a product is out of stock, users can pre-order — only logged in users.
  - After login, the system handles and stores previous guest saved products under their account.
- **Cart Panel**: View saved or pre-ordered products.
  - Select quantities, apply promo codes, see real-time order summary.
  - Static shipping cost (10,000 IQD), with free shipping over 60,000 IQD.
- **Checkout Flow**:
  1. **Shipping Info**: Auto-filled for logged-in users(non-loggedin users can access to cart-modal till they login).
  2. **Payment Method**:
     - **Cash on Delivery**
     - **FIB (First Iraqi Bank)** – pay via:
       - QR Code (scan with phone)
       - Enter code manually
       - Redirect to FIB mobile app (only works on mobile browser)
     - 15-minute timer to complete payment, else cancelled.
  3. **Review Step**: Confirm all info.
- **Contact Page**:
  - Guest users: Email, Name, Subject, Message.
  - Logged-in users: Just Subject & Message.

---

## 🔐 Authentication & Authorization

- **JWT Auth (stored in cookies)** for security.
- Token verification on every sensitive endpoint.
- Role-based control:
  - Unauthorized requests (e.g. posting product by non-admin) are blocked.
  - Refresh tokens & session logic handled on the backend.

---

## 🛠️ Admin Dashboard

### 🎩 Super Admin Features
- Access to all sections.
- View **full product edit history** (who/when/what).
- Assign tasks to admins, filter by status.
- Create/delete/update admins.
- View contact messages & who replied.

### 🧑‍💼 Admin Types & Permissions
- **Content Admin** → Manage blogs and informational content.
- **Product Admin** → Create, update, delete products. Product filter & tracking.
- **Sales Admin** → Handle incoming orders, update order statuses (Processing → Shipped → Completed).
- **Contact Admin** → View/respond to customer contact messages.
- **All Admins** → Access Task section, change task status.

---

## 📦 Orders & Notifications

- **Order Flow**:
  - Order status updated by admins (Processing → Shipped → Completed).
  - Customers can cancel before completion.
- **Notification System**:
  - Customers:
    - New blogs/products
    - Order status updates
    - Pre-ordered product refill alerts
    - Contact message replies
  - Admins:
    - New tasks
    - Contact messages
    - New orders
- All notifications are also emailed using **Nodemailer**.

---

## 📂 What This Repo Includes

- 🔹 Screenshots of every page/component/section.
- 🔹 This detailed `README.md`.
- 🔹 No source code – for IP protection and future commercial use.

---

## 🚀 Future Plans

- Public release as a production-ready SaaS or platform.
- Mobile App version (React Native or Flutter).
- Expand payment methods.
- Push notifications.


---

## 📫 Contact

For more info or opportunities to collaborate:

**Author**: Hemn raqib  
**Email**: hemnraqeeb02@gmail.com  

---

⭐ If you like the idea, feel free to star the repo and share feedback!
