# FinanceHub - Global Banking Platform

<div align="center">
  <img src="https://images.pexels.com/photos/6801648/pexels-photo-6801648.jpeg?auto=compress&cs=tinysrgb&w=1200&h=400&fit=crop" alt="FinanceHub Banner" width="100%" height="200" style="border-radius: 10px; object-fit: cover;">
  
  <h3>🌍 Modern Multi-Currency Banking Dashboard</h3>
  <p>A beautiful, responsive financial platform built with React, TypeScript, and Tailwind CSS</p>
  
  [![React](https://img.shields.io/badge/React-18.3.1-blue.svg)](https://reactjs.org/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-5.5.3-blue.svg)](https://www.typescriptlang.org/)
  [![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4.1-38B2AC.svg)](https://tailwindcss.com/)
  [![Framer Motion](https://img.shields.io/badge/Framer_Motion-10.16.16-ff69b4.svg)](https://www.framer.com/motion/)
  [![Vite](https://img.shields.io/badge/Vite-5.4.2-646CFF.svg)](https://vitejs.dev/)
</div>

## ✨ Features

### 🎨 **Modern Design System**
- **Dark/Light Theme Support** - Seamless theme switching with system preference detection
- **Glass Morphism UI** - Beautiful frosted glass effects and backdrop blur
- **Responsive Design** - Optimized for desktop, tablet, and mobile devices
- **Smooth Animations** - Powered by Framer Motion for delightful interactions

### 💰 **Financial Dashboard**
- **Multi-Currency Wallet** - Support for USD, EUR, GBP, JPY with real-time balances
- **Transaction Timeline** - Detailed transaction history with categories and locations
- **Live Exchange Rates** - Real-time currency exchange rates with bank comparisons
- **Portfolio Overview** - Comprehensive view of your global financial positions

### 🔧 **Technical Features**
- **TypeScript** - Full type safety and enhanced developer experience
- **Component Architecture** - Modular, reusable React components
- **Context API** - Efficient state management for themes and user preferences
- **Performance Optimized** - Lazy loading and optimized bundle size

## 🚀 Quick Start

### Prerequisites

Before you begin, ensure you have the following installed:
- **Node.js** (version 18.0 or higher)
- **npm** (version 8.0 or higher) or **yarn**
- **Git** for version control

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/financehub.git
   cd financehub
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` to see the application running.

## 📁 Project Structure

```
financehub/
├── public/                 # Static assets
├── src/
│   ├── components/        # React components
│   │   ├── CTAStrip.tsx          # Bottom call-to-action strip
│   │   ├── ExchangeRates.tsx     # Currency exchange rates
│   │   ├── Sidebar.tsx           # Navigation sidebar
│   │   ├── ThemeToggle.tsx       # Theme switching component
│   │   ├── TopBar.tsx            # Top navigation bar
│   │   ├── TransactionTimeline.tsx # Transaction history
│   │   └── WalletOverview.tsx    # Portfolio overview
│   ├── contexts/          # React contexts
│   │   └── ThemeContext.tsx      # Theme management
│   ├── App.tsx           # Main application component
│   ├── main.tsx          # Application entry point
│   └── index.css         # Global styles
├── tailwind.config.js    # Tailwind CSS configuration
├── vite.config.ts        # Vite configuration
└── package.json          # Project dependencies
```

## 🎯 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with hot reload |
| `npm run build` | Build the project for production |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run ESLint to check code quality |

## 🎨 Design System

### Color Palette

#### Dark Theme
- **Base**: `#0D1412` - Primary background
- **Surface**: `#1A1F1D` - Card backgrounds
- **Glass**: `rgba(255, 255, 255, 0.05)` - Glass morphism effects
- **Text**: `#E8E8E8` - Primary text color
- **Accent**: `#65A30D` - Brand green color

#### Light Theme
- **Base**: `#FAFAFA` - Primary background
- **Surface**: `#FFFFFF` - Card backgrounds
- **Glass**: `rgba(0, 0, 0, 0.05)` - Glass morphism effects
- **Text**: `#1A1A1A` - Primary text color
- **Accent**: `#65A30D` - Brand green color

### Typography
- **Primary Font**: Inter (Google Fonts)
- **System Fallback**: system-ui, -apple-system, BlinkMacSystemFont

## 🔧 Configuration

### Theme Configuration

The application supports three theme modes:
- **Light**: Traditional light theme
- **Dark**: Modern dark theme
- **System**: Automatically follows system preference

Theme preferences are automatically saved to localStorage and persist across sessions.

### Customizing Colors

To customize the color scheme, edit the `tailwind.config.js` file:

```javascript
theme: {
  extend: {
    colors: {
      'lime-accent': '#65A30D', // Change this to your brand color
      // Add more custom colors here
    }
  }
}
```

## 📱 Responsive Breakpoints

| Breakpoint | Width | Description |
|------------|-------|-------------|
| `sm` | 640px | Small devices |
| `md` | 768px | Medium devices |
| `lg` | 1024px | Large devices |
| `xl` | 1280px | Extra large devices |

## 🌟 Key Components

### WalletOverview
Displays multi-currency portfolio with:
- Total portfolio value
- Individual currency balances
- Performance indicators
- Balance visibility toggle

### TransactionTimeline
Shows recent transactions with:
- Transaction categorization
- Location and flag indicators
- Amount and currency display
- Interactive hover effects

### ExchangeRates
Provides real-time exchange rates featuring:
- Live currency pairs
- Bank rate comparisons
- Quick exchange calculator
- Performance charts

### Sidebar Navigation
Collapsible navigation with:
- Section switching
- User profile display
- Smooth animations
- Active state indicators

## 🚀 Deployment

### Build for Production

```bash
npm run build
```

This creates an optimized production build in the `dist` folder.

### Deploy to Netlify

1. **Build the project**
   ```bash
   npm run build
   ```

2. **Deploy to Netlify**
   - Drag and drop the `dist` folder to [Netlify Drop](https://app.netlify.com/drop)
   - Or connect your GitHub repository for automatic deployments

### Deploy to Vercel

```bash
npm install -g vercel
vercel --prod
```

## 🛠️ Development

### Adding New Components

1. Create a new file in `src/components/`
2. Follow the existing component structure
3. Use TypeScript interfaces for props
4. Include Framer Motion animations
5. Ensure responsive design

Example component structure:
```typescript
import React from 'react';
import { motion } from 'framer-motion';

interface ComponentProps {
  // Define your props here
}

export const YourComponent: React.FC<ComponentProps> = ({ }) => {
  return (
    <motion.div
      initial={{ opacity: 0 }}
      animate={{ opacity: 1 }}
      className="your-classes-here"
    >
      {/* Your component content */}
    </motion.div>
  );
};
```

### Code Style Guidelines

- Use TypeScript for all components
- Follow React functional component patterns
- Use Tailwind CSS for styling
- Include proper TypeScript interfaces
- Add meaningful animations with Framer Motion
- Ensure accessibility compliance

## 🤝 Contributing

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some amazing feature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **React Team** - For the amazing React framework
- **Tailwind CSS** - For the utility-first CSS framework
- **Framer Motion** - For smooth animations
- **Lucide React** - For beautiful icons
- **Vite** - For fast development experience
- **Pexels** - For high-quality stock photos

## 📞 Support

If you have any questions or need help with setup, please:

1. Check the [Issues](https://github.com/yourusername/financehub/issues) page
2. Create a new issue if your problem isn't already reported
3. Provide detailed information about your environment and the issue

---

<div align="center">
  <p>Made with ❤️ by [Your Name]</p>
  <p>⭐ Star this repository if you found it helpful!</p>
</div>