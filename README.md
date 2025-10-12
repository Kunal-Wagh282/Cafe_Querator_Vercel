# Cafe Querator

A modern music management system for cafes that integrates with Spotify, allowing cafe owners to manage music playlists and customers to request songs through table-specific interfaces.

## 🎵 Features

### For Cafe Owners (Dashboard)
- **Spotify Integration**: Connect your Spotify account to manage music
- **Table Management**: Visual table layout with real-time status tracking
- **Music Control**: Play, pause, skip tracks, and manage playlists
- **Queue Management**: Handle song requests from customers
- **Search & Add**: Search for songs and add them to playlists
- **Real-time Updates**: Live updates via WebSocket connections

### For Customers (Table Interface)
- **Song Requests**: Browse and request songs from your table
- **Live Queue**: See current queue and your request status
- **Table-specific Access**: Unique URLs for each table
- **Modern UI**: Clean, responsive interface optimized for mobile

## 🚀 Tech Stack

- **Frontend**: React 18 + Vite
- **Styling**: Tailwind CSS + Custom CSS
- **Routing**: React Router DOM
- **HTTP Client**: Axios
- **Music Integration**: Spotify Web Playback SDK
- **Real-time**: WebSocket connections
- **Animations**: Lottie animations
- **Notifications**: React Toastify
- **Icons**: FontAwesome + React Icons

## 📱 Pages & Routes

- `/` - Landing page (redirects based on auth status)
- `/login` - User authentication
- `/register` - User registration
- `/spotify-login` - Spotify OAuth integration
- `/dashboard` - Main cafe management interface
- `/:cafename/table/:tableid` - Customer table interface
- `/outh` - OAuth callback handler

## 🛠️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Cafe_Querator_Vercel
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment**
   - Update `src/config.js` with your backend API URLs
   - Set up Spotify app credentials for OAuth integration

4. **Start development server**
   ```bash
   npm run dev
   ```

5. **Build for production**
   ```bash
   npm run build
   ```

## 🔧 Configuration

The application uses a centralized config file (`src/config.js`) for API endpoints:

```javascript
const CONFIG = {
    API_URL: 'your-backend-api-url',
    CUSTOMER_URL: 'your-customer-api-url',
    QUEUE_URL: 'your-queue-management-url',
    WEBSOCKET_URL: 'your-websocket-url'
};
```

## 🎨 Key Components

- **Dashboard**: Main management interface with music controls
- **Table**: Customer-facing interface for song requests
- **SpotifyPlayer**: Custom Spotify player with progress tracking
- **Navbar**: Navigation component with user controls
- **Preloader**: Loading animations using Lottie
- **ConfirmationModal**: User confirmation dialogs

## 📦 Dependencies

### Core Dependencies
- React 18.3.1
- React Router DOM 6.26.2
- Axios 1.7.7
- React Spotify Web Playback 0.14.4

### UI & Styling
- Tailwind CSS 3.4.10
- FontAwesome 6.7.1
- React Icons 5.3.0
- React Toastify 10.0.6

### Development
- Vite 5.4.1
- ESLint 9.9.0
- PostCSS 8.4.41

## 🚀 Deployment

The project is configured for deployment on Vercel with SPA routing support via `vercel.json`.

## 📝 License

This project is private and proprietary.

## 🤝 Contributing

This is a private project. Please contact the maintainers for contribution guidelines.
