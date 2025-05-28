# ReduxCart

A simple shopping cart application built with React, Redux Toolkit, and Firebase as the backend. This project demonstrates state management with Redux, async actions, and integration with a Firebase Realtime Database.

## Features
- Add and remove products from the cart
- Cart state is persisted to Firebase
- Notifications for cart actions (success, error, pending)
- Modular component structure

## Project Structure
```
reduxCart/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── Cart/
│   │   ├── Layout/
│   │   ├── Shop/
│   │   └── UI/
│   ├── store/
│   ├── App.js
│   ├── index.js
│   └── index.css
├── package.json
└── README.md
```

## Getting Started

### Prerequisites
- Node.js (v16 or later recommended)
- npm (v8 or later)

### Installation
1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd reduxCart
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```

### Running the App
Start the development server:
```bash
npm start
```
The app will be available at [http://localhost:3000](http://localhost:3000).

## Firebase Backend
This project uses a Firebase Realtime Database for persisting cart data. The default database URL is hardcoded in `src/store/cart-action.js`:
```
https://redux-4bba3-default-rtdb.europe-west1.firebasedatabase.app/cart.json
```
If you want to use your own Firebase project:
1. Create a Firebase Realtime Database.
2. Replace the database URL in `src/store/cart-action.js` with your own endpoint.
3. (Optional) Refactor to use environment variables for better security.

## Scripts
- `npm start` – Start the development server
- `npm run build` – Build for production
- `npm test` – Run tests
- `npm run eject` – Eject from Create React App

## Dependencies
- React
- Redux Toolkit
- React Redux
- Firebase (REST API)

## License
This project is for educational purposes. 