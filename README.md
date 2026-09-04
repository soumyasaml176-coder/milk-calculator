# 🥛 Milk Rate Calculator

A comprehensive milk pricing calculator with support for **Pragati Milk Products** official pricing tables and multiple calculation models.

## Features

✨ **Pragati Pricing Tables** - Official W.E.F 21.05.2026 pricing data with bilinear interpolation
📊 **Multiple Models** - Switch between Pragati tables and formula-based calculations
🧮 **Smart Calculation** - Automatic lookup and interpolation for accurate pricing
💾 **History Tracking** - Persistent calculation history stored in browser
🎨 **Modern UI** - Beautiful gradient design with responsive layout
⚠️ **Validation** - Built-in term & condition checks (FAT < 3.2%, SNF < 7.5%)

## How to Use

1. **Select Pricing Model**
   - **Pragati**: Uses official pricing table (recommended)
   - **Formula**: Uses simple mathematical formula

2. **Enter Milk Parameters**
   - **FAT %**: Milk fat percentage (e.g., 4.50)
   - **SNF %**: Solids-Not-Fat percentage (e.g., 8.50)
   - **Quantity**: Amount of milk in liters (default: 1L)

3. **Calculate**
   - Click "Calculate Price" button
   - View rate per liter and total amount
   - History is auto-saved

## Pricing Models

### Pragati Model
- Based on official Pragati Milk Products pricing table
- Covers FAT range: 3.20% - 4.70%
- SNF range: 7.50% - 9.00%
- Uses bilinear interpolation for precise values
- Date: W.E.F 21.05.2026

### Formula Model
```
Rate = (FAT × 6.5) + (SNF × 1.8) - 0.05
```

## Terms & Conditions

❌ **No Payment if:**
- FAT < 3.2%
- SNF < 7.5%
- Adulterated milk

## Technical Details

- **Pure HTML/CSS/JavaScript** - No dependencies
- **Local Storage** - Calculation history saved in browser
- **Responsive Design** - Works on mobile and desktop
- **Pragati Data** - Complete pricing matrix embedded

## File Structure

```
milk-calculator/
├── index.html          # Complete calculator application
├── README.md           # This file
└── LICENSE             # MIT License
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/soumyasaml176-coder/milk-calculator.git
```

2. Open in browser:
```bash
cd milk-calculator
open index.html
```

Or access online if deployed.

## Pragati Pricing Table

The calculator includes the complete official pricing matrix from Pragati Milk Products:

| FAT % | SNF 7.50% | SNF 8.00% | SNF 8.50% | SNF 9.00% |
|-------|-----------|-----------|-----------|-----------|
| 3.20  | ₹34.29    | ₹36.27    | ₹38.05    | ₹39.46    |
| 4.00  | ₹37.69    | ₹39.67    | ₹41.58    | ₹43.42    |
| 4.70  | ₹40.65    | ₹42.57    | ₹44.55    | ₹46.39    |

*Full table embedded in calculator*

## Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## History Feature

- Stores up to 10 recent calculations
- Persistent across browser sessions
- Shows: FAT%, SNF%, Quantity, Rate, Total
- Clear history anytime

## Development

No build process required. Simply edit `index.html` and refresh.

### To add new pricing models:
1. Update the pricing data structure in JavaScript
2. Add selection option in the model dropdown
3. Update calculation logic

## License

MIT License - See LICENSE file

## Author

Created for Pragati Milk Products farmers and distributors

## Support

For issues or suggestions, please create an issue on GitHub.

---

**Last Updated:** September 4, 2026
**Data Source:** Pragati Milk Products W.E.F 21.05.2026
