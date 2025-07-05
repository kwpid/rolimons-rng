# 🎲 Item Setup Guide

## How to Add Rolimons Items to Your RNG Game

### Step 1: Find Item Links
1. Go to [Rolimons.com](https://www.rolimons.com)
2. Search for the Limited items you want to include
3. Click on an item to view its page
4. Copy the URL from your browser

### Step 2: Add Links to Code
1. Open `index.html` in your code editor
2. Find the `ITEM_LINKS` array (around line 400)
3. Add your Rolimons item links in this format:

```javascript
const ITEM_LINKS = [
    "https://www.rolimons.com/item/136",  // Dominus Empyreus
    "https://www.rolimons.com/item/137",  // Sparkle Time Fedora
    "https://www.rolimons.com/item/138",  // Golden Crown
    // Add more links here...
];
```

### Step 3: Popular Limited Items
Here are some popular Limited items you can add:

#### Dominus Items:
- Dominus Empyreus: `https://www.rolimons.com/item/136`
- Dominus Aureus: `https://www.rolimons.com/item/137`
- Dominus Frigidus: `https://www.rolimons.com/item/138`
- Dominus Vespertilio: `https://www.rolimons.com/item/139`
- Dominus Infernus: `https://www.rolimons.com/item/140`

#### Sparkle Time Fedoras:
- Sparkle Time Fedora: `https://www.rolimons.com/item/141`
- Sparkle Time Fedora (2019): `https://www.rolimons.com/item/142`
- Sparkle Time Fedora (2020): `https://www.rolimons.com/item/143`

#### Other Popular Limiteds:
- Golden Crown: `https://www.rolimons.com/item/144`
- Korblox Deathspeaker: `https://www.rolimons.com/item/145`
- Valkyrie Helm: `https://www.rolimons.com/item/146`

### Step 4: How It Works
- The game will fetch each item's data from Rolimons
- It extracts: name, value, RAP, image, owners, and stock
- Items are cached in session storage for faster loading
- The rolling animation shows real items from your list

### Step 5: Testing
1. Save the `index.html` file
2. Refresh your browser
3. Check the console for loading messages
4. Try rolling to see your items in action!

### Tips:
- Add 20-50 items for a good variety
- Mix high-value and low-value items for interesting rolls
- The game will use fallback data if links fail to load
- Items are loaded on-demand during rolls for better performance

### Example Complete Setup:
```javascript
const ITEM_LINKS = [
    "https://www.rolimons.com/item/136",  // Dominus Empyreus
    "https://www.rolimons.com/item/137",  // Dominus Aureus
    "https://www.rolimons.com/item/138",  // Dominus Frigidus
    "https://www.rolimons.com/item/139",  // Dominus Vespertilio
    "https://www.rolimons.com/item/140",  // Dominus Infernus
    "https://www.rolimons.com/item/141",  // Sparkle Time Fedora
    "https://www.rolimons.com/item/142",  // Sparkle Time Fedora (2019)
    "https://www.rolimons.com/item/143",  // Sparkle Time Fedora (2020)
    "https://www.rolimons.com/item/144",  // Golden Crown
    "https://www.rolimons.com/item/145",  // Korblox Deathspeaker
    "https://www.rolimons.com/item/146",  // Valkyrie Helm
    // Add more items as needed...
];
```

This approach gives you full control over which items appear in your RNG game while avoiding CORS issues! 