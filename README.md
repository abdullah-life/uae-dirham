# UAE Dirham Font - New Currency Symbol

A custom CSS font implementation for the **new UAE Dirham currency symbol**. Since the symbol isn't yet supported by Unicode, this font uses character mapping to display the official symbol.

## 🚀 Installation & Usage

### CDN Usage (Recommended)

**Setup:**
```css
@font-face { 
    font-family: 'Dirham'; 
    src: url('https://cdn.jsdelivr.net/gh/abdullah-life/uae-dirham@main/dirham-v1.5.ttf') format('truetype');
    font-display: swap;
    unicode-range: U+0044;
} 

.dirham { 
    font-family: 'Dirham', Arial, sans-serif;
}
```

**Using Class:**
```html
<span class="dirham">D</span> 1,250.00
```

**Using Inline CSS:**
```html
<span style="font-family: 'Dirham', Arial, sans-serif;">D</span> 1,250.00
```

### Local Installation

**Setup:**
1. **Download Font File:**
   - [Direct Download: dirham-v1.5.ttf](https://cdn.jsdelivr.net/gh/abdullah-life/uae-dirham@main/dirham-v1.5.ttf)
   - Or from [GitHub Releases](../../releases)
2. Place `dirham-v1.5.ttf` in your `assets/fonts/` directory
3. Add CSS:

```css
@font-face { 
    font-family: 'Dirham'; 
    src: url('./assets/fonts/dirham-v1.5.ttf') format('truetype');
    font-display: swap;
    unicode-range: U+0044;
}

.dirham { 
    font-family: 'Dirham', Arial, sans-serif;
}
```

**Using Class:**
```html
<span class="dirham">D</span> 1,250.00
```

**Using Inline CSS:**
```html
<span style="font-family: 'Dirham', Arial, sans-serif;">D</span> 1,250.00
```

## 🔧 Complete HTML Example

### CDN Version
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UAE Dirham Symbol</title>
    <style>
        @font-face { 
            font-family: 'Dirham'; 
            src: url('https://cdn.jsdelivr.net/gh/abdullah-life/uae-dirham@main/dirham-v1.5.ttf') format('truetype');
            font-display: swap;
            unicode-range: U+0044;
        }
        
        .dirham { 
            font-family: 'Dirham', Arial, sans-serif;
        }
        
        .price {
            font-size: 2rem;
            color: #00732F;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>UAE Dirham Symbol Examples</h1>
    
    <!-- Using CSS Class -->
    <p>Price: <span class="dirham">D</span> 1,250.00</p>
    
    <!-- Using Inline Style -->
    <p>Cost: <span style="font-family: 'Dirham', Arial, sans-serif;">D</span> 999.99</p>
    
    <!-- Large Price Display -->
    <div class="price">
        <span class="dirham">D</span> 299
    </div>
</body>
</html>
```

### Local Version
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UAE Dirham Symbol</title>
    <style>
        @font-face { 
            font-family: 'Dirham'; 
            src: url('./assets/fonts/dirham-v1.5.ttf') format('truetype');
            font-display: swap;
            unicode-range: U+0044;
        }
        
        .dirham { 
            font-family: 'Dirham', Arial, sans-serif;
        }
        
        .price {
            font-size: 2rem;
            color: #00732F;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>UAE Dirham Symbol Examples</h1>
    
    <!-- Using CSS Class -->
    <p>Price: <span class="dirham">D</span> 1,250.00</p>
    
    <!-- Using Inline Style -->
    <p>Cost: <span style="font-family: 'Dirham', Arial, sans-serif;">D</span> 999.99</p>
    
    <!-- Large Price Display -->
    <div class="price">
        <span class="dirham">D</span> 299
    </div>
</body>
</html>
```

### CSS Implementation
```css
/* Essential: Only 'D' inside this class becomes the symbol */
.dirham { 
    font-family: 'Dirham', Arial, sans-serif;
}

/* Large display for prices */
.price {
    font-size: 2rem;
}

.price .dirham {
    color: #00732F; /* UAE green */
    font-weight: bold;
}
```

## 🎨 Examples

### E-commerce Integration
```html
<!-- Product price -->
<div class="product-price">
    <span class="dirham">D</span> 299.99
</div>

<!-- Sale banner -->
<h2 class="sale-price">
    From <span class="dirham">D</span> 149
</h2>
```

### Financial Applications
```html
<!-- Account balance -->
<div class="balance">
    Balance: <span class="dirham">D</span> 12,485.50
</div>

<!-- Transaction list -->
<li class="transaction">
    Coffee Shop - <span class="dirham">D</span> 28.00
</li>
```

## ⚠️ Important Notes

- **Character Mapping**: Type `D` to display the new UAE Dirham symbol
- **Unicode Future**: Once Unicode officially supports the symbol, this mapping may change
- **Fallback Behavior**: Without the font, `D` displays as regular "D"
- **Selective Loading**: Font only affects the "D" character, other text remains normal

## 🌐 Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome  | 38+     | ✅ Full Support |
| Firefox | 39+     | ✅ Full Support |
| Safari  | 10+     | ✅ Full Support |
| Edge    | 79+     | ✅ Full Support |
| IE      | 11      | ⚠️ Limited Support |


## 📄 License

Available under the [SIL Open Font License 1.1](LICENSE) - free for commercial and personal use.

---

**Note**: This is a temporary solution until Unicode officially includes the new UAE Dirham symbol. If you have any suggestions or wants to make corrections, feel free to create an issue.
