# Qualia Design Tokens - Engineering Package

🚀 **Ready-to-use design tokens for Qualia engineering teams**

This package contains the core design tokens in formats optimized for engineering integration.

## 📦 What's Included

- **`qualia-tokens.css`** - CSS Custom Properties (CSS Variables)
- **`qualia-tokens.json`** - JSON format following W3C Design Tokens specification

## 🔧 Quick Integration

### Option 1: CSS Import
```css
@import 'qualia-tokens.css';

/* Use tokens in your styles */
.button {
  background-color: var(--interactive-primary);
  color: var(--text-inverse);
  padding: var(--spacing-md);
  border-radius: var(--border-radius-md);
}
```

### Option 2: JSON for Build Tools
```javascript
// Import tokens in JavaScript/TypeScript
import tokens from './qualia-tokens.json';

const primaryColor = tokens.tokens.interactive.primary.$value;
```

## 🎨 Token Categories

| Category | Description | Example Usage |
|----------|-------------|---------------|
| **Primitive** | Base colors, foundation | Building other tokens |
| **Brand** | Qualia brand colors | Primary actions, logos |
| **Semantic** | Meaning-based colors | Success, error, warning |
| **Interactive** | Button states & actions | Buttons, links, controls |
| **Surface** | Backgrounds & containers | Cards, modals, pages |
| **Text** | Typography colors | Headings, body, labels |
| **Spacing** | Layout & padding | Margins, padding, gaps |
| **Typography** | Font properties | Text styles, hierarchy |
| **Border Radius** | Corner rounding | Buttons, cards, inputs |

## 📋 Integration Checklist

- [ ] Include token file in build process
- [ ] Replace hardcoded values with tokens
- [ ] Test across all supported browsers
- [ ] Validate accessibility (contrast ratios)
- [ ] Update component library
- [ ] Document team usage patterns

## 🎯 Key Benefits

✅ **Consistency** - Single source of truth for design values  
✅ **Maintainability** - Update once, change everywhere  
✅ **Scalability** - Easy to extend and modify  
✅ **Accessibility** - WCAG compliant contrast ratios  
✅ **Developer Experience** - Clear naming and documentation  

## 🔄 Usage Examples

### Buttons
```css
.btn-primary {
  background: var(--interactive-primary);
  color: var(--text-inverse);
}

.btn-primary:hover {
  background: var(--interactive-primary-hover);
}
```

### Cards
```css
.card {
  background: var(--surface-card);
  border: 1px solid var(--surface-border);
  border-radius: var(--border-radius-lg);
  padding: var(--spacing-lg);
}
```

### Typography
```css
.heading {
  font-family: var(--font-family-primary);
  font-size: var(--font-size-2xl);
  font-weight: var(--font-weight-semibold);
  color: var(--text-primary);
}
```

## 🚫 Red Flags - Avoid These

❌ Using hardcoded colors: `color: #22C55E`  
✅ Use tokens instead: `color: var(--interactive-primary)`

❌ Using hardcoded spacing: `padding: 16px`  
✅ Use tokens instead: `padding: var(--spacing-md)`

❌ Mixing semantic meanings: Success color for error states  
✅ Use appropriate semantic tokens: `var(--semantic-error)`

## 📞 Support

**Questions?** Reach out to the Design Systems team:
- Slack: `#design-systems`
- Email: `design-systems@qualia.com`

---

**Version:** 1.0  
**Last Updated:** October 2024  
**Maintained by:** Design Systems Team