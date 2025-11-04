# 💰 Crypto Portfolio Tracker

A modern, feature-rich cryptocurrency portfolio tracking application built with vanilla JavaScript. Track your crypto investments with real-time prices from Binance, set profit/loss thresholds, and manage your portfolio with ease.

## 🌐 Live Demo

**[View Live Application](https://abdulrafayn001.github.io/crypto-portfolio-tracker/)**

## ✨ Features

### 📊 Portfolio Management
- **Add Investments**: Track multiple cryptocurrency purchases with detailed information
- **Edit Investments**: Modify existing investment details anytime
- **Delete Investments**: Remove investments with a beautiful confirmation modal
- **Real-time Price Updates**: Live cryptocurrency prices from Binance API (updates every 10 seconds)
- **Multiple Entries**: Add multiple purchases of the same coin at different prices

### 💹 Advanced Tracking
- **Profit/Loss Tracking**: Automatic calculation of gains/losses in both USD and percentage
- **Threshold Alerts**: Set custom profit or loss targets with two types:
  - **Percentage-based**: Get notified when your investment reaches a specific percentage gain/loss
  - **Price-based**: Get alerts when a coin reaches a target price
- **Purchase Date/Time**: Track when each investment was made for better analysis
- **Live Statistics**: View total invested amount, current value, and overall P&L at a glance

### 📥📤 Import/Export
- **Export to CSV**: Download your entire portfolio as a CSV file
- **Import from CSV**: Upload CSV files to populate your portfolio
- **Duplicate Prevention**: Smart detection prevents duplicate entries when importing
- **Multiple File Support**: Import from multiple CSV files - only unique data is added
- **Flexible CSV Format**: Supports various CSV formats as long as required columns are present

### 🎨 Modern UI/UX
- **Card-Based Layout**: Clean, modern card design for easy scanning
- **Responsive Design**: Fully responsive - works perfectly on desktop, tablet, and mobile
- **Purple Gradient Theme**: Beautiful gradient color scheme throughout
- **Hover Effects**: Smooth animations and transitions
- **Tooltips**: Helpful tooltips on action buttons
- **Icon Buttons**: Clean emoji icons for edit and delete actions

### 💾 Data Persistence
- **LocalStorage**: All data persists in browser's localStorage
- **Never Lose Data**: Your portfolio remains intact even after closing the browser
- **No Backend Required**: 100% client-side application
- **Privacy-Focused**: Your data stays on your device

### 🪙 Supported Cryptocurrencies
- Bitcoin (BTC), Ethereum (ETH), Binance Coin (BNB)
- XRP, Cardano (ADA), Dogecoin (DOGE), Solana (SOL)
- Polkadot (DOT), Polygon (MATIC), Litecoin (LTC)
- Shiba Inu (SHIB), Avalanche (AVAX), Uniswap (UNI)
- Chainlink (LINK), Cosmos (ATOM), Stellar (XLM)
- And 10+ more popular cryptocurrencies!
- **Searchable Dropdown**: Type to search and quickly find your coin

## 🚀 Getting Started

### Online (Easiest)
Simply visit the [live application](https://abdulrafayn001.github.io/crypto-portfolio-tracker/) and start tracking your investments immediately!

### Local Setup
1. Clone the repository:
```bash
git clone https://github.com/abdulrafayn001/crypto-portfolio-tracker.git
```

2. Navigate to the project directory:
```bash
cd crypto-portfolio-tracker
```

3. Open `index.html` in your web browser:
```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

That's it! No installation, no dependencies, no build process needed.

## 📖 How to Use

### Adding an Investment

1. **Select Coin**: Type or select the cryptocurrency from the dropdown
2. **Enter Quantity**: Specify how many coins you purchased
3. **Enter Buy Price**: Input the price you paid (in USDT)
4. **Set Date/Time**: Choose when you made the purchase (defaults to current date/time)
5. **Optional - Set Thresholds**: 
   - Choose threshold type (None, Percentage, or Price)
   - Set profit target (e.g., +10% or $50,000)
   - Set loss limit (e.g., -5% or $40,000)
6. **Click "Add Investment"**: Your investment is saved and portfolio updates instantly

### Editing an Investment

1. Click the **✏️ Edit** button on any investment card
2. Modify any fields in the modal
3. Click **"Save Changes"**
4. Your investment is updated immediately

### Deleting an Investment

1. Click the **🗑️ Delete** button on any investment card
2. Confirm deletion in the custom modal
3. Investment is permanently removed

### Exporting Your Portfolio

1. Click the **📤 Export** button in the portfolio header
2. A CSV file is automatically downloaded with filename: `crypto_portfolio_YYYY-MM-DD.csv`
3. Open with Excel, Google Sheets, or any spreadsheet application

### Importing Investments

1. Click the **📥 Import** button in the portfolio header
2. Select a CSV file from your computer
3. The app validates the format and imports unique entries
4. You'll see a summary: "Successfully imported X investment(s). Skipped Y duplicate(s)"

#### CSV Format Requirements

Your CSV file must include these columns (case-insensitive):
- **Symbol**: Cryptocurrency symbol (e.g., BTC, ETH)
- **Quantity**: Amount of coins
- **Buy Price**: Purchase price in USDT
- **Buy Date**: Date/time of purchase (ISO format)

Optional columns:
- **Threshold Type**: none, percentage, or price
- **Profit Threshold**: Target profit value
- **Loss Threshold**: Stop loss value

**Example CSV:**
```csv
Symbol,Quantity,Buy Price,Buy Date,Threshold Type,Profit Threshold,Loss Threshold
BTC,0.5,45000,2025-11-04T10:30:00.000Z,percentage,10,-5
ETH,2,3000,2025-11-03T14:20:00.000Z,none,,
SOL,10,120,2025-11-02T09:15:00.000Z,price,150,100
```

## 🔔 Threshold Alerts

The app monitors your investments and shows alerts when thresholds are reached:

- **🎯 Profit Target Reached**: Green alert when investment hits profit goal
- **⚠️ Loss Threshold Reached**: Yellow warning when investment reaches stop loss
- Alerts appear at the top of the page
- Auto-dismiss after 5 seconds

## 📱 Mobile Experience

The app is fully optimized for mobile devices:
- **Responsive Cards**: Full-width cards on small screens
- **Touch-Friendly**: Large tap targets for buttons
- **Stacked Layout**: Vertical layout for forms and buttons
- **No Horizontal Scroll**: Everything fits perfectly
- **Fast Loading**: Lightweight and optimized

## 🛠️ Technical Details

### Built With
- **HTML5**: Semantic markup
- **CSS3**: Modern styling with flexbox and grid
- **Vanilla JavaScript**: No frameworks or libraries
- **Binance API**: Real-time cryptocurrency prices
- **LocalStorage API**: Client-side data persistence

### Browser Compatibility
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Opera (latest)

### API Integration
The app uses the [Binance Public API](https://binance-docs.github.io/apidocs/spot/en/) to fetch real-time cryptocurrency prices:
- Endpoint: `https://api.binance.com/api/v3/ticker/price`
- No API key required
- Updates every 10 seconds
- Supports all major cryptocurrencies paired with USDT

## 🎯 Use Cases

- **Personal Investment Tracking**: Monitor your crypto portfolio performance
- **Tax Reporting**: Export data for tax purposes
- **Investment Analysis**: Track profit/loss over time
- **Risk Management**: Set stop-loss alerts
- **Portfolio Diversification**: Visualize your holdings
- **Historical Tracking**: Maintain records of all purchases

## 🔒 Privacy & Security

- **No Account Required**: No sign-up, no login
- **Local Data Only**: All data stored in your browser
- **No Server Communication**: Except for price fetching from Binance
- **No Tracking**: No analytics or tracking scripts
- **Open Source**: Full transparency - inspect the code yourself

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/AmazingFeature`
3. **Commit your changes**: `git commit -m 'Add some AmazingFeature'`
4. **Push to the branch**: `git push origin feature/AmazingFeature`
5. **Open a Pull Request**

### Ideas for Contribution
- Add more cryptocurrency options
- Implement dark mode
- Add charts and graphs
- Create portfolio analytics dashboard
- Add multi-currency support
- Implement data backup to cloud services

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [Binance API](https://binance-docs.github.io/apidocs/spot/en/) for real-time cryptocurrency data
- Emoji icons from native Unicode support
- Inspired by the need for a simple, privacy-focused portfolio tracker

## 📞 Contact & Support

- **GitHub**: [@abdulrafayn001](https://github.com/abdulrafayn001)
- **Issues**: [Report bugs or request features](https://github.com/abdulrafayn001/crypto-portfolio-tracker/issues)
- **Live Demo**: [https://abdulrafayn001.github.io/crypto-portfolio-tracker/](https://abdulrafayn001.github.io/crypto-portfolio-tracker/)

## 🎉 Features Coming Soon

- 📊 Interactive charts and graphs
- 🌙 Dark mode support
- 📧 Email notifications for threshold alerts
- 💱 Multi-currency support (EUR, GBP, etc.)
- 📈 Historical price data
- 🔄 Auto-refresh interval customization
- 💾 Cloud backup option
- 📱 Progressive Web App (PWA) support

---

**Made with ❤️ by [Abdul Rafay](https://github.com/abdulrafayn001)**

**⭐ Star this repository if you find it helpful!**
