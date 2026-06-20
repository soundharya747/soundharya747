# SpendTracker - Ionic App

A mobile-first personal finance app built with Ionic Web Components, HTML5, CSS3, and Chart.js.

## Features
- 📊 **Home Dashboard** – Monthly summary, recent transactions, quick actions
- 💳 **Transactions Screen** – All/Sent/Received tabs, search, filter by vendor/date
- 💰 **Budget Tracking** – Category budgets with progress bars, 80% alerts, exceeded warnings
- 📈 **Insights** – Donut chart by category, 6-month bar trend, top merchants, savings rate
- ➕ **Add Transaction** – Manual entry with category, type (debit/credit), payment method
- 📱 **SMS Auto-read banner** – Enable/disable automatic SMS transaction detection

## How to Run

### Option 1: Open Directly
Just open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge).

### Option 2: Local Server (recommended for full PWA experience)
```bash
# Python
python3 -m http.server 8080

# Node.js
npx serve .

# Then open: http://localhost:8080
```

### Option 3: Convert to Native App with Capacitor
```bash
npm install -g @ionic/cli
npm install @capacitor/core @capacitor/cli @capacitor/android @capacitor/ios
npx cap init SpendTracker com.spendtracker.app
npx cap add android
npx cap add ios
npx cap copy
npx cap open android   # Opens in Android Studio
npx cap open ios       # Opens in Xcode
```

## Tech Stack
- **Ionic Web Components** v7 (CDN) – UI components & icons
- **Ionicons** v7 – Icon library
- **Chart.js** v4 – Donut & bar charts
- **Vanilla JS** – No build step required

## Screens
| Screen | Description |
|--------|-------------|
| Home | Overview, recent 5 transactions, quick action buttons |
| Transactions | Full list with search & tab filters |
| Budget | Category-wise budget progress with alerts |
| Insights | Visual charts + merchant analytics |

## Customization
All transaction data is in the `transactions` array in `index.html`.
Budget limits are in the `budgets` array.
Categories with icons and colors are in the `categories` array.
