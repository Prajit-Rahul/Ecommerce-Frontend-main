# Ecommerce Frontend

React storefront for a full-stack ecommerce application with category browsing, authentication flows, cart management, and Stripe-based checkout.

This project pairs with the Spring Boot backend in [Ecommerce-Backend-main](https://github.com/Prajit-Rahul/Ecommerce-Backend-main).

## What It Includes

- Category-based shopping experience
- Product cards and collection views
- Sign in and sign up pages
- Redux-managed cart state
- Quantity updates inside the cart overlay
- Stripe checkout integration
- React Router-based navigation across storefront pages

## Tech Stack

- React 18
- React Router
- Redux and Redux Thunk
- Material UI
- Axios / Fetch
- Stripe

## Main Routes

- `/home`: landing page
- `/shops`: category-driven storefront
- `/signup`: authentication page
- `/contact`: contact page
- `/hats`, `/sneakers`, `/jackets`, `/womens`, `/mens`: collection pages

## Project Structure

- `src/Components/home`: landing page UI
- `src/Components/shop`: storefront and category listing
- `src/Components/card` and `src/Components/card-list`: product display
- `src/Components/authentication`, `login`, `signup`: auth flow
- `src/Components/cart-items`: cart overlay and checkout interaction
- `src/Components/redux`: async data fetching and cart state management

## Backend Integration

The frontend fetches category and user data from the paired backend API and is designed to work with:

- category endpoints under `/api/category`
- user registration under `/api/user/registration`

## Running Locally

```bash
npm install
npm start
```

The app runs with Create React App defaults. Start the backend separately so storefront and registration requests can resolve correctly.

## Why This Repo Matters

This repo shows practical frontend application work beyond static pages: stateful UI, API integration, checkout flow, and a modular component structure for an end-to-end shopping experience.
