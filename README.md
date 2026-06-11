# Bitcoin Current Price

## 📋 Description
A web application that displays the current Bitcoin price in real-time. This project demonstrates API integration with cryptocurrency data providers and provides users with up-to-date Bitcoin market information.

## 🎯 Objective
- Fetch real-time Bitcoin price data
- Display current market price
- Show price trends and history
- Implement currency conversion
- Create an interactive user interface
- Demonstrate API integration skills

## ✨ Features
- **Real-time Price Display**
  - Current Bitcoin price
  - Multiple currency support
  - Live price updates
  - Price change percentage
  - Market data

- **Price Information**
  - Historical prices
  - 24-hour high/low
  - Market cap
  - Trading volume
  - Circulating supply

- **Visualizations**
  - Price charts
  - Trend indicators
  - Market performance
  - Price history graphs

- **Currency Conversion**
  - USD, EUR, GBP support
  - Real-time conversion
  - Custom currency selection
  - Exchange rates

## 🛠️ Technologies Used
- **Frontend**
  - HTML5
  - CSS3
  - JavaScript (ES6+)

- **APIs**
  - CoinGecko API (free)
  - Cryptocurrency APIs

- **Libraries** (if used)
  - Chart.js - Price charts
  - Fetch API - HTTP requests

## 📁 Project Structure
```
bitcoin.github.io/
├── index.html
├── css/
│   ├── style.css
│   ├── responsive.css
│   └── theme.css
├── js/
│   ├── app.js
│   ├── api.js
│   └── utils.js
├── images/
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Web browser (modern version)
- Text editor or IDE
- Internet connection

### Installation

1. Clone the repository
```bash
git clone https://github.com/RahulKirtoniya/bitcoin.github.io.git
cd bitcoin.github.io
```

2. Open in browser
```bash
# Using Python
python -m http.server 8000

# Or open index.html directly
```

3. Access the application
```
http://localhost:8000
```

## 💻 Usage

### View Current Price
1. Open the application
2. See Bitcoin price displayed prominently
3. View in default currency

### Change Currency
1. Click currency dropdown
2. Select desired currency
3. Price updates automatically

### View Charts
1. Navigate to Charts section
2. Select time period
3. View price history

### Market Data
1. Check 24-hour stats
2. View market cap
3. See trading volume

## 🔌 API Integration

### CoinGecko API
```javascript
// Get current Bitcoin price
GET https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd

// Get market data
GET https://api.coingecko.com/api/v3/coins/bitcoin

// Get price history
GET https://api.coingecko.com/api/v3/coins/bitcoin/market_chart?vs_currency=usd&days=365
```

### API Response Example
```json
{
  "bitcoin": {
    "usd": 42850.50,
    "eur": 39500.25,
    "gbp": 34200.75
  }
}
```

## 📊 Key JavaScript Functions

```javascript
// Fetch Bitcoin price
async function getBitcoinPrice() { }

// Convert currency
function convertCurrency(price, currency) { }

// Display price
function displayPrice(price) { }

// Get market data
async function getMarketData() { }

// Draw price chart
function drawChart(data) { }
```

## 🎨 UI Components
- Price display card
- Currency selector
- Price charts
- Market statistics
- 24-hour stats
- Market cap display
- Volume information

## 📱 Responsive Design
- Mobile-first approach
- Tablet optimization
- Desktop experience
- Cross-browser support

### Breakpoints
- Desktop: 1200px+
- Tablet: 768px - 1199px
- Mobile: <768px

## 💱 Supported Currencies
- USD (US Dollar)
- EUR (Euro)
- GBP (British Pound)
- JPY (Japanese Yen)
- INR (Indian Rupee)
- AUD (Australian Dollar)
- CAD (Canadian Dollar)
- SGD (Singapore Dollar)

## 📈 Price Information Displayed
```
Current Price: $42,850.50
24h Change: +2.5% ↑
24h High: $43,200
24h Low: $41,500
Market Cap: $850 Billion
Volume: $25 Billion
Circulating Supply: 21 Million BTC
```

## 🔐 Security Features
- API key handling (if needed)
- CORS compliance
- Input validation
- Error handling

## ⚠️ Limitations
- Free tier rate limits
- No real-time socket connection
- Delayed updates (5-60 minutes)
- No user authentication
- No historical data storage

## 🚀 Future Enhancements
- Real-time WebSocket updates
- Multiple cryptocurrencies
- Price alerts
- User favorites
- Portfolio tracking
- Price predictions
- Technical analysis
- Social sentiment
- News integration
- Mobile app
- Dark mode
- Advanced charting tools

## 🎓 Learning Concepts
- Fetch API and AJAX
- Async/Await
- DOM manipulation
- CSS Grid and Flexbox
- Responsive design
- API integration
- Error handling
- Data visualization
- Chart.js usage

## 📝 Code Examples

### Fetch Price
```javascript
async function getBitcoinPrice() {
  try {
    const response = await fetch(
      'https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd'
    );
    const data = await response.json();
    return data.bitcoin.usd;
  } catch (error) {
    console.error('Error:', error);
  }
}
```

### Display Price
```javascript
function displayPrice(price) {
  const priceElement = document.getElementById('price');
  priceElement.textContent = `$${price.toFixed(2)}`;
}
```

### Draw Chart
```javascript
function drawChart(dates, prices) {
  const ctx = document.getElementById('myChart').getContext('2d');
  new Chart(ctx, {
    type: 'line',
    data: {
      labels: dates,
      datasets: [{
        label: 'Bitcoin Price',
        data: prices,
        borderColor: 'rgb(255, 153, 0)',
        tension: 0.1
      }]
    }
  });
}
```

## 🐛 Troubleshooting

### Price Not Loading
- Check internet connection
- Verify API is accessible
- Check browser console for errors
- Clear browser cache

### Chart Not Displaying
- Verify Chart.js is loaded
- Check data format
- Verify canvas element exists

### Currency Conversion Issues
- Check currency code
- Verify API supports currency
- Clear cache and reload

## 🔗 Useful Resources
- [CoinGecko API Docs](https://www.coingecko.com/en/api)
- [Chart.js Documentation](https://www.chartjs.org/)
- [Fetch API Guide](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- [Bitcoin Info](https://bitcoin.org/)

## 👨‍💻 Author
**Rahul Kirtoniya**

## 📄 License
Open source - feel free to use for educational purposes

## 🙏 Credits
- Price data: CoinGecko
- Charts: Chart.js
- Icons: Font Awesome

## 🤝 Contributing
Contributions are welcome! Please submit pull requests for improvements.

---

**Track Bitcoin Price in Real-Time! ₿**