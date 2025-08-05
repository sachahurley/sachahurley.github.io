# Betterfly FTUX - iPhone Home Screen Component

This project contains a React component that recreates an iPhone home screen in dark mode, generated from the Figma design.

## Features

- 📱 Pixel-perfect iPhone home screen layout
- 🌙 Dark mode gradient background
- 📋 All standard iOS app icons with emoji placeholders
- 🔍 Search field with blur effect
- 📲 Bottom dock with 4 main apps
- ⚡ Built with React and Tailwind CSS

## Quick Start

### Option 1: Simple HTML File (Recommended for demo)

1. Open `index.html` in your browser
2. The component will load automatically using CDN resources

### Option 2: Development Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start development server:
   ```bash
   npm run dev
   ```

3. Open your browser to the provided localhost URL

## Project Structure

```
betterfly-ftux/
├── components/
│   └── HomeScreen.js          # Main iPhone home screen component
├── index.html                 # Demo page
├── package.json              # Project dependencies
├── tailwind.config.js        # Tailwind CSS configuration
├── postcss.config.js         # PostCSS configuration
└── README.md                 # This file
```

## Component Usage

The main component is `IPhoneHomeScreenDark` which can be used in any React application:

```jsx
import { IPhoneHomeScreenDark } from './components/HomeScreen.js';

function App() {
  return (
    <div className="w-screen h-screen flex items-center justify-center bg-black">
      <div className="w-[393px] h-[852px] relative overflow-hidden">
        <IPhoneHomeScreenDark />
      </div>
    </div>
  );
}
```

## Customization

- **App Icons**: Replace the emoji placeholders in the `appIcons` object with actual app icons
- **Background**: Modify the gradient in `imgModeDark` variable
- **Colors**: Update the Tailwind config for custom color schemes
- **Layout**: Adjust positioning and spacing in the component structure

## Design System

The component follows iOS design patterns:
- SF Pro font family
- iOS-standard app icon radius (14px)
- Proper spacing and proportions
- Backdrop blur effects for glassmorphism
- iOS color palette

## Browser Support

- Modern browsers with CSS backdrop-filter support
- React 18+ compatibility
- Tailwind CSS 3+ features

## License

MIT License - feel free to use in your projects!