# Splitter -- Smart Expense Sharing App

Splitter is a modern, elegant, and fully client‑side web application for
tracking shared expenses and calculating fair settlements among groups.
Built using **JavaScript**, **Vite**, and **TailwindCSS**, it provides a
smooth UI and accurate settlement logic powered by a clean service‑based
architecture.

------------------------------------------------------------------------

## 🚀 Features

### 👥 User Management

-   Add users dynamically\
-   Import/export full user data\
-   Validates duplicate or empty entries

### 💵 Expense Tracking

-   Add expenses with:
    -   Payer
    -   Amount
    -   Description\
-   Clean UI with animated list items\
-   Real‑time visual updates

### 🔄 Smart Settlement Algorithm

-   Splits expenses evenly across all users\
-   Computes net balances\
-   Simplifies transactions using a greedy settle‑up algorithm\
-   Displays "who owes whom" clearly

### 📁 Import & Export

-   Export all users + expenses as a `.json` file\
-   Import previously exported files\
-   Automatically reconstructs UI from imported data

### 🎨 Modern UI & UX

-   Beautiful animations\
-   Gradient background\
-   Responsive forms\
-   Toast notifications\
-   Smooth scrolling containers

------------------------------------------------------------------------

## 🧱 Project Structure

    .
    ├── index.html
    ├── index.css
    ├── src/
    │   ├── main.js
    │   ├── models/
    │   │   ├── user.js
    │   │   └── expense.js
    │   ├── services/
    │   │   ├── userService.js
    │   │   ├── expenseService.js
    │   │   └── storageService.js
    │   ├── ui/
    │   │   ├── expenseUI.js
    │   │   └── domHelpers.js
    │   └── utils/
    │       └── toastUtil.js
    ├── package.json
    └── vite.config.js

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   **Vite** -- blazing‑fast frontend tooling\
-   **TailwindCSS v4** -- styling & utility classes\
-   **JavaScript ES Modules**\
-   **Toastify.js** -- notifications\
-   **Lucide Icons**

------------------------------------------------------------------------

## 📦 Installation & Local Development

Make sure you have **Node.js (v16+)** installed.

``` bash
# Install dependencies
npm install

# Start dev server
npm run dev
```

App will be available at:

    http://localhost:3001

------------------------------------------------------------------------

## 📤 Build for Production

``` bash
npm run build
```

Your optimized bundle will be created by Vite.

To preview the production build:

``` bash
npm run preview
```

------------------------------------------------------------------------

## 📚 Core Concepts

### 👉 UserService

Handles creation, validation, and storage of user objects using a `Map`.

### 👉 ExpenseService

Tracks all expenses and calculates simplified settlements.

### 👉 StorageService

Manages JSON export/import with structure validation.

### 👉 ExpenseUI

Connects DOM events to services and updates the interface.

------------------------------------------------------------------------

## 🔐 Data Format

### Exported JSON example:

``` json
{
  "users": [
    { "id": "uuid", "name": "Alice" }
  ],
  "expenses": [
    { "id": "uuid", "paidBy": "Alice", "amount": 25, "description": "Snacks" }
  ],
  "exportDate": "2025-01-01T10:00:00.000Z"
}
```

------------------------------------------------------------------------

## 🤝 Contributing

Contributions are welcome!\
Feel free to submit issues or pull requests.

------------------------------------------------------------------------

## 📄 License

Distributed under the **MIT License**.\
See `LICENSE` for details.

------------------------------------------------------------------------

## ❤️ Acknowledgements

-   Icons by [Lucide](https://lucide.dev)
-   Notifications by Toastify
-   Powered by Vite + Tailwind
