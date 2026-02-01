# 🕒 Time Clock App

[![Live Demo](https://img.shields.io/badge/demo-live-success)](https://tbb1031.github.io/clockinapp/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PWA](https://img.shields.io/badge/PWA-enabled-orange.svg)](https://web.dev/progressive-web-apps/)

A beautiful, modern time tracking web application designed for employees and small businesses. Track work hours effortlessly with an elegant dark-themed interface, offline support, and powerful export capabilities.

![Time Clock App](https://img.shields.io/badge/Built%20with-HTML%20%7C%20CSS%20%7C%20JavaScript-blue)

## ✨ Features

### ⏱️ Time Tracking
- **Quick Clock In/Out**: One-click time tracking with real-time clock display
- **Manual Entry**: Add time logs retroactively with custom dates and times
- **Smart Duration Calculation**: Automatic calculation of hours worked, handles overnight shifts

### 📊 Data Management
- **Venue Tracking**: Log work at multiple venues (First Avenue, Fine Line, 7th Street Entry, Palace Theatre)
- **Position Management**: Track different job positions (Tickets, Door, Exit Door)
- **Local Storage**: All data stored locally in your browser for privacy and offline access
- **Export Options**: 
  - CSV format for universal compatibility
  - Excel (.xlsx) format with formatted columns
  - Timestamped file names for easy organization

### 📈 Analytics
- **Visual Dashboard**: Dedicated analytics page with insights
- **Work History**: Complete log of all clock in/out events
- **Hours Summary**: Track total hours worked per shift

### 🎨 User Experience
- **Modern Dark Theme**: Beautiful gradient design with glassmorphic cards
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Progressive Web App (PWA)**: Install on your device for a native app experience
- **Offline Support**: Continue tracking time without internet connection
- **Real-time Clock**: Always-visible current time display

## 🚀 Live Demo

**Try it now:** [https://tbb1031.github.io/clockinapp/](https://tbb1031.github.io/clockinapp/)

## 🛠️ Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Custom CSS with CSS Variables, Flexbox, Grid
- **Icons**: Unicode emoji icons
- **Storage**: Browser LocalStorage API
- **Excel Export**: [SheetJS (xlsx)](https://sheetjs.com/) library
- **Fonts**: [Inter](https://fonts.google.com/specimen/Inter) from Google Fonts
- **PWA**: Web App Manifest, Service Worker ready

## 📦 Installation

### Option 1: Use the Live Demo
Simply visit [https://tbb1031.github.io/clockinapp/](https://tbb1031.github.io/clockinapp/) and start using the app immediately.

### Option 2: Install as PWA
1. Visit the live demo on a supported browser (Chrome, Edge, Safari)
2. Look for the "Install" button in your browser's address bar
3. Click "Install" to add the app to your home screen/app drawer
4. Launch the app anytime from your device like a native application

### Option 3: Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/TBB1031/clockinapp.git
   cd clockinapp
   ```

2. Open the app:
   - Simply open `index.html` in your web browser
   - Or use a local server:
     ```bash
     # Python 3
     python -m http.server 8000
     
     # Python 2
     python -m SimpleHTTPServer 8000
     
     # Node.js (with http-server)
     npx http-server
     ```

3. Navigate to `http://localhost:8000` in your browser

## 📖 Usage Guide

### Quick Clock In/Out

1. **Clock In**: Click the "Clock In" button when starting work
2. **Clock Out**: Click the "Clock Out" button when finishing work
3. The app automatically calculates hours worked and saves the entry

### Manual Time Entry

Perfect for adding past shifts or corrections:

1. **Select Date**: Choose the work date
2. **Enter Venue**: Select or type the venue name
3. **Set Times**: Enter start and end times
4. **Choose Position**: Select your job role
5. **Add Entry**: Click "Add Log Entry" to save

### Viewing Logs

- All entries appear in the "Recent Logs" section
- Each log shows: Venue name, Position, Date, Time In, Time Out, and Hours Worked

### Exporting Data

- **Excel**: Click "Excel" for a formatted .xlsx file
- **CSV**: Click "CSV" for a comma-separated values file
- **Clear**: Click "Clear" to delete all logs (with confirmation)

### Analytics Dashboard

Click the "Analytics" tab to view:
- Work history visualizations
- Total hours calculations
- Performance insights

## 🔧 Development

### Project Structure

```
clockinapp/
├── index.html          # Main time entry page
├── analytics.html      # Analytics dashboard
├── manifest.json       # PWA configuration
├── README.md           # Documentation
└── .gitmodules         # Git submodules (if any)
```

### Key Features Implementation

- **Time Calculation**: Handles overnight shifts by detecting negative duration
- **Data Persistence**: Uses `localStorage` for client-side data storage
- **Export Functionality**: 
  - CSV: Native JavaScript implementation
  - Excel: SheetJS library integration
- **PWA**: Configured via `manifest.json` with app icons

### Customization

#### Adding More Venues
Edit the datalist in `index.html`:
```html
<datalist id="Venue">
  <option value="Your Venue Name"></option>
</datalist>
```

#### Adding More Positions
Edit the select options in `index.html`:
```html
<select id="job">
  <option value="Your Position">Your Position</option>
</select>
```

#### Changing Theme Colors
Modify CSS variables in the `:root` section:
```css
:root {
  --primary-blue: #6495ed;
  --accent-cyan: #4dd8ff;
  /* ... more colors */
}
```

## 🌐 Deployment

### GitHub Pages (Recommended)

1. Go to your repository **Settings** → **Pages**
2. Under "Build and deployment", set:
   - **Source**: GitHub Actions
3. Push to the `main` branch to trigger automatic deployment
4. Your app will be available at: `https://yourusername.github.io/clockinapp/`

### Other Hosting Options

The app is a static website and can be deployed to:
- **Netlify**: Drag and drop the folder
- **Vercel**: Import from GitHub
- **Cloudflare Pages**: Connect your repository
- **Any static hosting**: Upload the files via FTP/SFTP

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### Ideas for Contributions
- Add more analytics visualizations
- Implement data backup/restore features
- Add support for multiple users
- Create a backend integration option
- Improve accessibility features
- Add internationalization (i18n)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [Inter Font](https://rsms.me/inter/) by Rasmus Andersson
- [SheetJS](https://sheetjs.com/) for Excel export functionality
- Inspired by modern time tracking tools

## 📧 Contact

For questions or feedback, please open an issue on GitHub.

---

**Made with ❤️ for easy time tracking**