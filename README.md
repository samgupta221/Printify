# 🎨 Printify – AI Print-on-Demand Platform

> An AI-powered Print-on-Demand platform built with the MERN stack, allowing users to generate artwork with AI, customize products using a visual editor, create listings, preview designs on apparel mockups, and complete purchases through Stripe.

## 🚀 Overview

**Printify** is a full-stack AI-powered Print-on-Demand application built using **MongoDB, Express.js, React, and Node.js**.

The platform provides an end-to-end workflow for creating and selling custom apparel:

**AI Artwork → Design Editor → Product Mockup → Listing → Checkout → Order Management**

Users can generate custom artwork from prompts, place designs on products, create listings, and purchase customized products through an integrated Stripe checkout.

---

## ✨ Features

### 🔐 Authentication

* Email/password authentication
* Secure session management with Better Auth
* Protected application routes
* Cookie-based authentication
* JWT plugin support
* Google OAuth support available in the original implementation

### 🤖 AI Artwork Generation

* Generate custom artwork from text prompts
* AI prompt engineering for Print-on-Demand designs
* Artwork generation integrated into the listing workflow
* Artwork uploaded and managed through Cloudinary

### 🎨 Design Editor

* Interactive product design editor
* Drag-and-drop design elements
* Canvas-based editing using Fabric.js
* Product mockup preview
* Design positioning and customization
* Real-time visual editing

### 👕 Product System

* T-shirts
* Hoodies
* Multiple product colors
* Product templates
* Product catalog
* Product detail pages
* Product mockups

### 🛍️ Listings

* Create custom product listings
* Add generated artwork to products
* Custom listing titles and descriptions
* Product previews
* Listing detail pages
* Listing management

### 💳 Payments

* Stripe Checkout integration
* Secure payment flow
* Stripe webhook handling
* Order creation after successful payment

### 📦 Orders

* User order history
* Order details
* Product information
* Order amount and status
* Payment-based order processing

### 🖼️ Image Processing

* Cloudinary image uploads
* Background removal support using Remove.bg API
* Product mockup generation
* Artwork management

### 📱 Responsive UI

* Modern dashboard
* Responsive layout
* Sidebar navigation
* Mobile-friendly components
* Toast notifications
* Reusable UI components

---

## 🛠️ Tech Stack

### Frontend

| Technology           | Purpose                 |
| -------------------- | ----------------------- |
| React 19             | UI development          |
| TypeScript           | Type safety             |
| Vite                 | Frontend tooling        |
| React Router         | Routing                 |
| TanStack React Query | Server-state management |
| Axios                | API communication       |
| Fabric.js            | Design canvas/editor    |
| Tailwind CSS         | Styling                 |
| Radix UI             | UI primitives           |
| Better Auth          | Authentication          |
| Lucide React         | Icons                   |
| Sonner               | Notifications           |

### Backend

| Technology  | Purpose            |
| ----------- | ------------------ |
| Node.js     | Runtime            |
| Express.js  | REST API           |
| TypeScript  | Type safety        |
| MongoDB     | Database           |
| Mongoose    | MongoDB ODM        |
| Better Auth | Authentication     |
| Cloudinary  | Image storage      |
| Stripe      | Payments           |
| AI SDK      | AI integration     |
| bcryptjs    | Password hashing   |
| Zod         | Validation         |
| Nodemon     | Development server |

---

## 📁 Project Structure

```text
MERN-AI-Print-OnDemand-Platform-main/
│
├── client/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── hooks/
│   │   ├── layout/
│   │   ├── lib/
│   │   ├── pages/
│   │   │   ├── auth/
│   │   │   ├── design/
│   │   │   ├── home/
│   │   │   ├── listings/
│   │   │   ├── orders/
│   │   │   └── settings/
│   │   ├── routes/
│   │   ├── types/
│   │   ├── App.tsx
│   │   └── main.tsx
│   │
│   ├── package.json
│   └── vite.config.ts
│
├── backend/
│   ├── src/
│   │   ├── assets/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── lib/
│   │   ├── middlewares/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── script/
│   │   ├── utils/
│   │   ├── validators/
│   │   ├── webhooks/
│   │   └── index.ts
│   │
│   ├── package.json
│   └── tsconfig.json
│
├── .gitignore
├── README.md
└── TECHWITHEMMA-LICENSE.md
```

---

# 🧠 Application Workflow

```text
                 ┌─────────────────┐
                 │      User       │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Authentication  │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Product Catalog │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ AI Artwork Gen. │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │  Design Editor  │
                 │    Fabric.js    │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Create Listing  │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Stripe Checkout │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │     Order       │
                 └─────────────────┘
```

---

# 🎨 Main Application Pages

### Home

Product discovery and featured products.

### Listings

Browse available custom products.

### Design Studio

Create and customize artwork using the interactive editor.

### Listing Details

View a product, design, colors, and pricing before purchasing.

### Orders

View previously placed orders and order information.

### Settings

Manage account/application settings.

---
