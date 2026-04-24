# Infosphere Club Hub

Infosphere Club Hub is a modern, dynamic web application designed to act as a centralized platform for managing and discovering various student clubs, their coordinators, members, events, and announcements. 

Built with React and Vite, it utilizes a lightweight backend architecture powered by Google Sheets and CSV parsing, providing an easy-to-update data source without needing a traditional database setup.

## ✨ Features

- **Club Directory:** Browse all available clubs and view detailed information for each.
- **Member & Coordinator Profiles:** Discover the people driving the clubs, from members to key coordinators.
- **Events & Announcements:** Stay updated with the latest events and important announcements across all clubs.
- **Performance Optimized:** Uses React's `lazy` and `Suspense` for code-splitting and faster initial page loads.
- **Serverless Data Fetching:** Seamlessly fetches and caches data from published Google Sheets (CSV) using `PapaParse` and `React Query`.
- **Responsive & Animated UI:** Smooth transitions and modern UI components powered by `Framer Motion` and CSS Modules.

## 🛠️ Tech Stack

- **Frontend Framework:** [React 18](https://react.dev/) + [Vite](https://vitejs.dev/)
- **Routing:** [React Router v6](https://reactrouter.com/)
- **Data Fetching & Caching:** [@tanstack/react-query](https://tanstack.com/query/latest)
- **Data Parsing:** [PapaParse](https://www.papaparse.com/) (for Google Sheets CSV parsing)
- **Animations:** [Framer Motion](https://www.framer.com/motion/)
- **Styling:** CSS Modules & Vanilla CSS
- **Icons:** [React Icons](https://react-icons.github.io/react-icons/)

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd infosphere-club-hub
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure Environment Variables:
   Create a `.env` file in the root directory and configure your Google Sheet CSV URLs. (Refer to the `googleSheetsAPI.js` service for expected data formats).

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:5173`.

## 📂 Project Structure

```text
src/
├── assets/          # Static assets like global CSS, images
├── components/      # Reusable UI components (layout, home, ui, etc.)
├── hooks/           # Custom React hooks (e.g., useFetchData)
├── pages/           # Lazy-loaded page components (Home, Clubs, Events, etc.)
├── services/        # API and data fetching logic (Google Sheets API)
├── App.jsx          # Main application routing and QueryClient setup
└── main.jsx         # React application entry point
```

## 📜 Scripts

- `npm run dev`: Starts the local Vite development server.
- `npm run build`: Bundles the application for production.
- `npm run preview`: Previews the production build locally.
- `npm run lint`: Runs ESLint to check for code quality and style issues.
