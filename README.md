# Eventful Frontend - Pure HTML/CSS/JavaScript

A beautiful, modern event ticketing platform frontend built with vanilla HTML, CSS (TailwindCSS), and JavaScript.

## 🎨 Features

- ✅ Pure HTML/CSS/JavaScript (No build process required!)
- ✅ TailwindCSS via CDN for beautiful styling
- ✅ Responsive design (mobile-friendly)
- ✅ Authentication (Login/Register)
- ✅ Event browsing and filtering
- ✅ Modern UI with gradients and animations
- ✅ Toast notifications
- ✅ No dependencies or npm install needed

## 🚀 Quick Start

### Option 1: Using Docker (Recommended)

```bash
# From project root
docker-compose up -d
```

Frontend will be available at: http://localhost:3001

### Option 2: Local Development

Simply open `index.html` in your browser, or use a simple HTTP server:

```bash
# Python
python -m http.server 3001

# Node.js (if you have it)
npx serve -p 3001

# PHP
php -S localhost:3001
```

Then visit: http://localhost:3001

## 📁 Structure

```
frontend/
├── index.html          # Home page
├── login.html          # Login page
├── register.html       # Registration page
├── events.html         # Browse events
├── css/
│   └── styles.css      # Custom styles
└── js/
    ├── config.js       # API configuration
    ├── auth.js         # Authentication functions
    └── main.js         # Main JavaScript functions
```

## 🎯 Pages

- **index.html** - Landing page with hero section and featured events
- **login.html** - User login
- **register.html** - User registration (Creator or Eventee)
- **events.html** - Browse and filter all events

## ⚙️ Configuration

Edit `js/config.js` to change API settings:

```javascript
const API_BASE_URL = "http://localhost:3000/api/v1";
const PAYSTACK_PUBLIC_KEY = "pk_test_your_key_here";
```

## 🎨 Customization

### Change Colors

Edit the TailwindCSS config in HTML files:

```javascript
tailwind.config = {
	theme: {
		extend: {
			colors: {
				primary: {
					// Your custom colors
				},
			},
		},
	},
};
```

### Add Custom Styles

Edit `css/styles.css` for custom CSS.

## 🌐 API Integration

The frontend connects to the backend API at `http://localhost:3000/api/v1`.

Make sure the backend is running before using the frontend.

## 📱 Responsive Design

The frontend is fully responsive and works on:

- Desktop (1920px+)
- Laptop (1024px+)
- Tablet (768px+)
- Mobile (320px+)

## 🔧 No Build Process!

One of the best features - there's no build process needed! Just:

1. Edit HTML/CSS/JS files
2. Refresh your browser
3. See changes instantly

## 🎉 That's It!

Your frontend is ready to use. Just open `index.html` or run it through Docker!
