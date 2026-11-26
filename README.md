# TechCam Online Store

A beginner-friendly e-commerce website built by a team of 7 members.

## Tech Stack

- [Vue 3](https://vuejs.org/) (JavaScript)
- [Vite](https://vitejs.dev/)
- [Vue Router](https://router.vuejs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- localStorage (for cart and wishlist)

## Features

- Homepage with Navbar, Hero Banner, Categories, Popular Products and Footer
- Shop page with Product Cards, Categories and Search
- Product Details page
- Shopping Cart (add, remove, change quantity, total price)
- Wishlist
- Login, Register and My Account pages
- Demo Checkout with order confirmation
- Responsive design (mobile and desktop)

## Getting Started

### Requirements

- [Node.js](https://nodejs.org/) 18 or newer
- [Git](https://git-scm.com/)

### Installation

```bash
git clone https://github.com/ThearithL/TechCam-online-store.git
cd TechCam-online-store
npm install
npm run dev
```

Open the link shown in the terminal, usually `http://localhost:5173`.

### Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start the development server |
| `npm run build` | Build the project for production |
| `npm run preview` | Preview the production build |

## Project Structure

```
TechCam-online-store/
├── public/
├── src/
│   ├── assets/          # Images, logo
│   ├── components/      # Reusable components (Navbar, Footer, ProductCard)
│   ├── data/            # Sample data (products.js)
│   ├── router/
│   │   └── index.js     # All routes
│   ├── views/           # One file per page
│   ├── App.vue
│   ├── main.js
│   └── style.css
├── index.html
├── package.json
└── vite.config.js
```

## Routes

| Page | Route | File |
|---|---|---|
| Home | `/` | `HomeView.vue` |
| Shop | `/shop` | `ShopView.vue` |
| Product Details | `/product/:id` | `ProductDetailsView.vue` |
| Cart | `/cart` | `CartView.vue` |
| Wishlist | `/wishlist` | `WishlistView.vue` |
| Login | `/login` | `LoginView.vue` |
| Register | `/register` | `RegisterView.vue` |
| My Account | `/account` | `AccountView.vue` |
| Checkout | `/checkout` | `CheckoutView.vue` |
| Order Success | `/order-success` | `OrderSuccessView.vue` |
| Not Found (404) | `/:pathMatch(.*)*` | `NotFoundView.vue` |

## Team

| Member | Role | Responsibility |
|---|---|---|
| 1 | Team Leader | Project plan, GitHub repo, router setup, merging code, deployment |
| 2 | UI/UX Designer | Logo, colors, fonts, Figma design |
| 3 | Homepage Developer | Homepage, Navbar, Hero Banner, Footer |
| 4 | Product Developer | Shop page, Product Card, Search, Product Details |
| 5 | Shopping Cart Developer | Cart, Wishlist, localStorage |
| 6 | Customer & Checkout Developer | Login, Register, My Account, Checkout |
| 7 | Tester & Documentation | Testing report, documentation, screenshots |

## Git Workflow

1. Pull the latest code before you start working:
   ```bash
   git pull origin main
   ```
2. Create your own branch:
   ```bash
   git checkout -b member-3-home
   ```
3. Work only on your own files to avoid conflicts.
4. Commit and push your branch:
   ```bash
   git add .
   git commit -m "Add homepage hero banner"
   git push origin member-3-home
   ```
5. Open a Pull Request on GitHub. The Team Leader reviews and merges it.

## Notes

- This is a demo project. Login, checkout and orders are not connected to a real backend or payment system.
- Cart and wishlist data are saved in the browser's localStorage.
- If you deploy to GitHub Pages, use `createWebHashHistory()` in the router to avoid 404 errors on refresh.
