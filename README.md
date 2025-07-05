# 🎲 Rolimons RNG Game

A modern, dark-themed RNG (Random Number Generator) game that uses real Roblox Limiteds data from the Rolimons API.

## Features

### 🎯 Main Game
- **Rolling Animation**: Smooth spinning animation when rolling for items
- **Value-Weighted Probability**: Items with higher values have lower chances (1 in 50 per 100 value)
- **Best Rolls Tracking**: Automatically tracks and displays rolls worth 250K+ value
- **Real-time Data**: Uses live data from Rolimons API

### 📦 Inventory Tab
- **Complete Item Database**: Shows all available Limiteds from Rolimons
- **Item Details**: Displays name, value, RAP, stock, and image
- **Stock Logic**: If an item has 250 or fewer owners, owners = stock
- **Responsive Grid**: Modern card-based layout

### 📊 Chances Tab
- **Probability Display**: Shows roll chances for each item
- **Value-Based Calculation**: 50% chance system (1 in 50 per 100 value)
- **Sorted by Value**: Items displayed from highest to lowest value

## Technical Features

### 🌐 CORS Handling
- Uses CORS proxy to handle API requests
- Robust error handling for network issues
- Graceful fallbacks for failed requests

### 🎨 Modern UI/UX
- **Dark Mode**: GitHub-inspired dark theme
- **Responsive Design**: Works on desktop and mobile
- **Smooth Animations**: Hover effects and transitions
- **Tab Navigation**: Clean tab-based interface

### 📱 Responsive Layout
- Grid-based layouts that adapt to screen size
- Mobile-friendly design
- Optimized for all devices

## How to Use

1. **Open the Game**: Simply open `index.html` in your web browser
2. **Start Rolling**: Click the "🎲 Roll for Items!" button on the Main tab
3. **View Results**: See your rolled item with all its details
4. **Track Progress**: Check the Best Rolls section for high-value items
5. **Explore Inventory**: Switch to the Inventory tab to browse all available items
6. **Check Chances**: Use the Chances tab to see probability for each item

## API Integration

The game integrates with the Rolimons API to fetch:
- Item names and images
- Current values and RAP (Recent Average Price)
- Stock information
- Owner counts

## Stock Logic

The game implements the specified stock logic:
- If an item has 250 or fewer owners → Stock = Owners
- Example: If an item has 26 owners, its stock is 26
- For items with more than 250 owners, uses actual stock data

## Chance Calculation

Roll chances are calculated based on item value:
- Formula: 1 in (Value ÷ 50)
- Example: Item worth 100 = 1 in 2 chance
- Example: Item worth 1000 = 1 in 20 chance
- Minimum chance is 1 in 1 (no decimals)

## Browser Compatibility

- Modern browsers with ES6+ support
- Chrome, Firefox, Safari, Edge
- Mobile browsers supported

## Setup

No installation required! Just:
1. Download the `index.html` file
2. Open it in any modern web browser
3. Start playing immediately

The game handles all API calls and CORS issues automatically.

## Note

This game uses a CORS proxy to access the Rolimons API. For production use, you may want to set up your own proxy server or use a different CORS solution. 