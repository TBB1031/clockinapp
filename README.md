# 🕒 Time Clock App

A beautiful, modern time tracking web application for employees with analytics and export capabilities.

## ✨ Features

### Quick Clock In/Out
- **One-click time tracking**: Instantly clock in and out with a single button press
- **Real-time clock display**: Live time display to track your current work session
- **Automatic time calculation**: Automatically calculates hours worked

### Manual Time Entry
- **Flexible data entry**: Add time logs manually for any date
- **Venue selection**: Choose from predefined venues or add custom ones
  - First Avenue
  - Fine Line
  - 7th Street Entry
  - Palace Theatre
- **Position tracking**: Select from different job positions (Tickets, Door, Exit Door)
- **Smart validation**: Ensures all required fields are filled before submission

### Analytics Dashboard
- **Visual insights**: Beautiful analytics page showing work patterns
- **Hours tracking**: Track total hours worked over different time periods
- **Venue breakdown**: See which venues you work at most frequently
- **Position analysis**: Understand time distribution across different roles

### Export Capabilities
- **CSV Export**: Download your time logs in CSV format for spreadsheet applications
- **Excel Export**: Export directly to Excel (.xlsx) format with formatted columns
- **Automatic file naming**: Files are named with current date for easy organization

### Progressive Web App (PWA)
- **Install on any device**: Add to home screen on mobile or desktop
- **Offline capability**: Works without internet connection using local storage
- **Native app experience**: Full-screen mode with no browser UI
- **Fast loading**: Optimized for instant loading and smooth performance

### Data Persistence
- **Local storage**: All data saved locally in your browser
- **No account required**: No sign-up or login needed
- **Privacy first**: Your data never leaves your device
- **Automatic saves**: Changes are saved instantly

## 🚀 Live Demo

**Try it now:** [https://tbb1031.github.io/clockinapp/](https://tbb1031.github.io/clockinapp/)

## 🛠️ Technology Stack

- **HTML5**: Modern semantic markup
- **CSS3**: Advanced styling with CSS variables and gradients
- **JavaScript**: Vanilla JavaScript (no frameworks required)
- **SheetJS**: Excel file generation
- **Local Storage API**: Client-side data persistence
- **PWA APIs**: Service workers and manifest for installable app experience

## 📦 Installation

### Using the Hosted Version
Simply visit [https://tbb1031.github.io/clockinapp/](https://tbb1031.github.io/clockinapp/) in your web browser.

### Installing as PWA
1. Visit the app in Chrome, Edge, or Safari
2. Click the install button in your browser's address bar
3. The app will be added to your home screen/applications
4. Launch like any native app

### Local Development
1. Clone the repository:
   ```bash
   git clone https://github.com/TBB1031/clockinapp.git
   cd clockinapp
   ```

2. Open `index.html` in your web browser:
   ```bash
   # Using Python's built-in server
   python -m http.server 8000
   
   # Or using Node.js
   npx http-server
   ```

3. Navigate to `http://localhost:8000` in your browser

## 💻 Usage

### Quick Clock In/Out
1. Open the app
2. Click **"Clock In"** when you start your shift
3. The button will become disabled and **"Clock Out"** will be enabled
4. Click **"Clock Out"** when you finish
5. Your time entry will be automatically logged with the current date

### Manual Time Entry
1. Navigate to the **Data Entry** tab
2. Select the date you worked
3. Enter or select the venue
4. Enter your start time (Time In)
5. Enter your end time (Time Out)
6. Select your position
7. Click **"Add Log Entry"**

### Viewing Analytics
1. Click the **Analytics** tab
2. View your work statistics including:
   - Total hours worked
   - Most frequent venues
   - Position breakdown
   - Time trends

### Exporting Data
1. Scroll to the **Recent Logs** section
2. Click **"CSV"** to export as comma-separated values
3. Click **"Excel"** to export as Microsoft Excel format
4. Files are automatically downloaded with current date in filename

### Clearing Data
1. In the Recent Logs section, click **"Clear"**
2. Confirm the action
3. All log entries will be permanently deleted

## 🔧 Configuration

### Customizing Venues
Edit the `index.html` file to add your own venues:

```html
<datalist id="Venue">
  <option value="Your Venue Name"></option>
  <!-- Add more venues here -->
</datalist>
```

### Customizing Positions
Modify the position dropdown in `index.html`:

```html
<select id="job">
  <option value="Your Position">Your Position</option>
  <!-- Add more positions here -->
</select>
```

## 📱 Browser Compatibility

- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🌐 Deployment

### GitHub Pages Setup
1. Go to repository **Settings → Pages**
2. Under "Build and deployment", select Source: **GitHub Actions**
3. Commit and push changes to the `main` branch
4. The workflow will automatically build and deploy your app
5. Access your app at: `https://[username].github.io/clockinapp/`

### Manual Deployment
Simply upload all files to any static web hosting service:
- Netlify
- Vercel
- AWS S3 + CloudFront
- Any traditional web host

## 📄 Data Structure

Time logs are stored in the browser's local storage with the following structure:

```javascript
{
  name: "Venue Name",
  job: "Position",
  timeInISO: "2026-01-31T14:00:00.000Z",
  timeOutISO: "2026-01-31T22:00:00.000Z",
  timeInFormatted: "02:00 PM",
  timeOutFormatted: "10:00 PM",
  hours: "8.00",
  date: "1/31/2026"
}
```

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👥 Author

**TBB1031**
- GitHub: [@TBB1031](https://github.com/TBB1031)

## 🐛 Issues

Found a bug or have a feature request? Please [open an issue](https://github.com/TBB1031/clockinapp/issues).

## ⭐ Support

If you find this project helpful, please give it a star on GitHub!