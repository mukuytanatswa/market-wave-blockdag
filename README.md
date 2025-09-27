# Wave Market Vision

AI-powered market prediction app with real-time data integration and investment analysis.

## Features

- 🔮 **AI Predictions**: Advanced technical analysis with bullish/bearish predictions
- 📊 **Real-time Data**: Live cryptocurrency, stock, and forex data
- 💰 **Investment Analysis**: Get detailed analysis for any asset
- 📈 **Interactive Charts**: Seamless historical-to-prediction chart transitions
- 🎯 **Multi-Asset Support**: Cryptocurrencies, stocks, forex, and commodities

## Tech Stack

- **Frontend**: React + TypeScript + Vite
- **UI**: Tailwind CSS + shadcn/ui
- **Charts**: Recharts
- **APIs**: CoinGecko, Alpha Vantage, AlphaWave

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/mukuytanatswa/wave-market-vision.git
cd wave-market-vision
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Environment Variables

Copy the example environment file and add your API keys:

```bash
cp env.example .env
```

Edit `.env` and add your API keys:

```env
# Alpha Vantage API Key (for stock and forex data)
VITE_ALPHA_VANTAGE_API_KEY=your_alpha_vantage_api_key_here

# AlphaWave API Key (if you have one)
VITE_ALPHAWAVE_API_KEY=your_alphawave_api_key_here

# CoinGecko API Key (optional, for higher rate limits)
VITE_COINGECKO_API_KEY=your_coingecko_api_key_here

# Metals API Key (for commodities data)
VITE_METALS_API_KEY=your_metals_api_key_here
```

### 4. Run the Development Server

```bash
npm run dev
```

## API Keys Setup

### Getting API Keys

1. **Alpha Vantage** (Free): <https://www.alphavantage.co/support/#api-key>
2. **CoinGecko** (Free): <https://www.coingecko.com/en/api>
3. **Metals API** (Free): <https://metals-api.com/>

### GitHub Secrets (for deployment)

If you're deploying to GitHub Pages, Vercel, or Netlify, add these as environment variables:

1. Go to your repository settings
2. Navigate to "Secrets and variables" → "Actions"
3. Add the following secrets:
   - `VITE_ALPHA_VANTAGE_API_KEY`
   - `VITE_ALPHAWAVE_API_KEY`
   - `VITE_COINGECKO_API_KEY`
   - `VITE_METALS_API_KEY`

## Usage

### Investment Analyzer

1. Enter any asset symbol (BTC, AAPL, EURUSD, etc.)
2. Select the asset type (Crypto, Stock, Forex, Commodity)
3. Choose a timeframe (1D, 1W, 1M, 3M)
4. Click "Analyze Investment" to get detailed predictions

### Supported Assets

- **Cryptocurrencies**: BTC, ETH, ADA, SOL, MATIC, DOT, LINK, UNI, and more
- **Stocks**: AAPL, MSFT, GOOGL, TSLA, AMZN, META, NVDA, NFLX, and more
- **Forex**: EURUSD, GBPUSD, USDJPY, AUDUSD, USDCAD, USDCHF, and more
- **Commodities**: Gold, Silver, Oil, and more

## Features

### Real-time Data

- Live cryptocurrency prices from CoinGecko
- Stock market data from Alpha Vantage
- Forex exchange rates
- Commodity prices

### AI Predictions

- Technical analysis using RSI, moving averages, and volatility
- Bullish/bearish trend predictions
- Confidence scoring
- Support and resistance levels

### Interactive Charts

- Historical price data
- Seamless prediction overlays
- Color-coded trend indicators
- Responsive design

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License - see LICENSE file for details

## Support

If you encounter any issues, please open an issue on GitHub.

---

**Note**: This app is for educational and informational purposes only. Always do your own research before making investment decisions.

## Deployment (GitHub Pages)

This project is configured to deploy to GitHub Pages using the `gh-pages` package. The build uses a repo-relative base so assets load correctly from GitHub Pages.

Quick steps:

1. Ensure this repo is pushed to GitHub under the name `market-wave-blockdag` (or update the `base` in `vite.config.ts` to match your repo name).
2. Install deps and run the deploy script:

```bash
npm install
npm run deploy
```

After the deploy completes, your site will be available at:

https://<your-github-username>.github.io/market-wave-blockdag/

Replace `<your-github-username>` with your GitHub username or organization. You can also view the GitHub Pages URL on your repository's Settings → Pages page after deployment.
