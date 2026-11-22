# PlantNet

## Project Overview
PlantNet is a full-stack plant marketplace and management web application designed to connect plant buyers, sellers, and administrators on a single platform. Users can browse plants, inspect detailed plant listings, place orders through a guided checkout modal, manage seller inventories, and monitor platform-wide user roles and statistics through a role-based dashboard.

---

## Technologies Used
- **Frontend:** React, Vite, Tailwind CSS, ESLint
- **Authentication & Client Services:** Firebase Authentication, Axios (`useAxiosSecure`)
- **Backend:** Node.js (`server/index.js`)
- **Architecture:** Component-based client (`client/`) and RESTful server (`server/`) with role-based route protection (`PrivateRoute`, `SellerRoute`, `AdminRoute`)

---

## Key Features
- **Storefront & Plant Details:** Browse all available plants on the home catalog (`Plants`, `Card`) and view full product details on `PlantDetails`.
- **Authentication & Role-Based Access:** Secure sign-up and login (`SignUp`, `Login`) powered by `AuthProvider`, `useAuth`, and `useRole` to separate **Customer**, **Seller**, and **Admin** access.
- **Customer Dashboard & Ordering:**
  - Purchase plants via `PurchaseModal` and `CheckoutForm`.
  - Track personal order history in `MyOrders`.
  - Request seller status via `BecomeSellerModal`.
- **Seller Inventory & Order Management:**
  - Add new plants (`AddPlant`, `AddPlantForm`).
  - Update or remove existing plant listings (`MyInventory`, `UpdatePlantModal`, `UpdatePlantForm`, `DeleteModal`).
  - Manage incoming customer orders (`ManageOrders`).
- **Admin Control Panel & Analytics:**
  - Manage users and assign/update roles (`ManageUsers`, `UpdateUserModal`).
  - View platform metrics and visual charts (`AdminStatistics`, `Chart`).
- **Responsive Shared UI:** Reusable `Navbar`, `Sidebar` (role-specific menus), `Footer`, `Profile`, `LoadingSpinner`, `EmptyState`, and `ErrorPage`.

---

## Your Contribution
- Designed and implemented the full-stack architecture separating `client` (React + Vite) and `server` (Node.js).
- Developed interactive dashboard modules, modals, and forms for plant listing CRUD operations, order checkout, and admin statistics.
- Structured responsive UI components using Tailwind CSS.


## How to Run

### Prerequisites
- **Node.js** (v18 or higher) and **npm** installed
- A configured **Firebase** project

### 1. Clone the Repository
```bash
git clone [https://github.com/UMMEKULSUMNICE/PlantNet.git](https://github.com/UMMEKULSUMNICE/PlantNet.git)
cd PlantNet
