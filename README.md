# Frontend - URL Shortener

A secure, client-side URL Shortener application built with React and Material UI 

## Features

### Core Functionality
- **URL Shortening**: Create shortened URLs with up to 5 URLs at once
- **Custom Shortcodes**: Optional custom shortcodes (3-20 alphanumeric characters)
- **Validity Management**: Default 30-minute validity with custom duration (1 minute to 24 hours)
- **Client-side Redirection**: All short URLs resolve via React Router
- **Data Persistence**: Uses localStorage for data persistence between sessions

### User Experience
- **Material UI Design**: Modern, responsive interface using Material UI components
- **Error Handling**: Comprehensive client-side validation with user-friendly error messages
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Accessibility**: Built with accessibility best practices

## Technology Stack

- **React 19.1.1**: Modern React with hooks
- **Material UI**: Complete UI component library
- **React Router**: Client-side routing and navigation
- **localStorage**: Data persistence
- **Custom Logging**: Replaces console.log usage as per requirements

## Project Structure

```
src/
├── components/
│   ├── URLShortener.jsx     
│   ├── Statistics.jsx       
│   └── RedirectHandler.jsx  
├── utils/
│   ├── logger.js            
│   ├── storage.js           
│   └── urlUtils.js          
├── App.jsx                  
└── main.jsx                 
```

## Key Features Implementation

### Custom Logging Middleware
- Replaces all `console.log` usage as required
- Stores logs in localStorage for persistence
- Supports different log levels (INFO, WARN, ERROR, DEBUG)
- Automatic log rotation to prevent memory overflow

### Data Models
- **URL Data**: Original URL, shortcode, creation/expiry timestamps, validity period
- **Analytics Data**: Click timestamps, referrer info, location data, user agent
- **Storage Keys**: Organized storage with cleanup functionality

## Usage

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Start Development Server**:
   ```bash
   npm run dev
   ```

3. **Access Application**:
   - Open browser to `http://localhost:5173`
   - Use the URL Shortener page to create shortened URLs
   - View statistics and analytics on the Statistics page

