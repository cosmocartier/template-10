# Format Archive - Digital Design Asset Marketplace

A modern, high-performance e-commerce platform for digital design assets built with Next.js 15, React 19, and GSAP animations.

## 🎨 Overview

Format Archive is a curated marketplace for digital design assets including mockups, graphic elements, and creative resources. The platform features smooth animations, modern UI/UX, and a seamless shopping experience for creative professionals.

## ✨ Features

### Core Functionality
- **E-commerce Platform**: Complete product catalog with shopping cart
- **Product Management**: Mockups, graphic elements, and design assets
- **Shopping Cart**: Persistent cart with local storage
- **Product Details**: Multiple image views and detailed product information
- **Responsive Design**: Optimized for all device sizes

### Technical Features
- **Modern Animations**: GSAP-powered smooth transitions and effects
- **Page Transitions**: View Transitions API for seamless navigation
- **State Management**: Zustand for efficient state handling
- **Performance**: Optimized with Next.js 15 and React 19
- **Smooth Scrolling**: Lenis integration for enhanced scrolling experience

### User Experience
- **Preloader**: Animated loading screen with counter
- **Smooth Navigation**: Custom page transitions
- **Product Previews**: Interactive product showcases on homepage
- **Modern UI**: Clean, professional design aesthetic

## 🛠️ Tech Stack

- **Framework**: Next.js 15.3.1 (App Router)
- **Frontend**: React 19.0.0
- **Styling**: CSS Modules + Global CSS
- **Animations**: GSAP 3.12.7 + @gsap/react 2.1.2
- **State Management**: Zustand 5.0.3
- **Smooth Scrolling**: Lenis 1.3.1
- **Page Transitions**: next-view-transitions 0.3.4
- **Text Animation**: split-type 0.3.4
- **Package Manager**: pnpm (recommended) / npm / yarn

## 📁 Project Structure

```
format-archive/
├── src/
│   ├── app/                    # Next.js App Router pages
│   │   ├── archive/           # Archive section
│   │   ├── catalogue/         # Product catalog
│   │   │   └── [slug]/       # Individual product pages
│   │   ├── editorial/         # Editorial content
│   │   ├── info/             # Information pages
│   │   ├── globals.css       # Global styles
│   │   ├── index.css         # Homepage styles
│   │   ├── layout.js         # Root layout
│   │   └── page.jsx          # Homepage
│   ├── components/           # Reusable components
│   │   ├── Cart/            # Shopping cart components
│   │   ├── Footer/          # Footer component
│   │   ├── Menu/            # Navigation menu
│   │   └── StoreProvider/   # State management
│   ├── store/               # Zustand stores
│   │   └── useCartStore.js  # Shopping cart state
│   ├── articles.js          # Editorial content data
│   ├── products.js          # Product catalog data
│   ├── utils.js             # Utility functions
│   └── client-layout.js     # Client-side layout wrapper
├── public/                  # Static assets
│   ├── product_images/      # Product images
│   └── hero.gif            # Homepage hero animation
├── package.json            # Dependencies and scripts
├── next.config.mjs         # Next.js configuration
└── jsconfig.json          # JavaScript configuration
```

## 🚀 Getting Started

### Prerequisites

- **Node.js**: Version 18.17 or higher
- **Package Manager**: pnpm (recommended), npm, or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd format-archive
   ```

2. **Install dependencies**
   ```bash
   # Using pnpm (recommended)
   pnpm install
   
   # Or using npm
   npm install
   
   # Or using yarn
   yarn install
   ```

3. **Run the development server**
   ```bash
   # Using pnpm
   pnpm dev
   
   # Or using npm
   npm run dev
   
   # Or using yarn
   yarn dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000) to view the application.

## 📦 Available Scripts

```bash
# Development
pnpm dev          # Start development server
pnpm build        # Build for production
pnpm start        # Start production server
pnpm lint         # Run ESLint

# Package Manager Commands
pnpm install      # Install dependencies
pnpm add <pkg>    # Add new dependency
pnpm remove <pkg> # Remove dependency
```

## 🌐 Deployment

### Vercel (Recommended)

1. **Install Vercel CLI**
   ```bash
   npm i -g vercel
   ```

2. **Deploy to Vercel**
   ```bash
   vercel
   ```

3. **Follow the prompts** to connect your repository and deploy.

### Other Platforms

#### Netlify
1. Connect your repository to Netlify
2. Set build command: `npm run build`
3. Set publish directory: `.next`
4. Deploy

#### Railway
1. Connect your repository to Railway
2. Set build command: `npm run build`
3. Set start command: `npm start`
4. Deploy

#### DigitalOcean App Platform
1. Connect your repository
2. Set build command: `npm run build`
3. Set run command: `npm start`
4. Deploy

### Environment Variables

Create a `.env.local` file for local development:

```env
# Add any environment variables here
NEXT_PUBLIC_SITE_URL=http://localhost:3000
```

For production, set environment variables in your hosting platform's dashboard.

## 🔧 Configuration

### Next.js Configuration (`next.config.mjs`)

```javascript
/** @type {import('next').NextConfig} */
const nextConfig = {
  // Add custom configuration here
};

export default nextConfig;
```

### JavaScript Configuration (`jsconfig.json`)

```json
{
  "compilerOptions": {
    "paths": {
      "@/*": ["./src/*"]
    }
  }
}
```

## 📱 Features in Detail

### Shopping Cart System
- **Persistent Storage**: Cart data saved in localStorage
- **Add/Remove Items**: Full CRUD operations
- **Quantity Management**: Increment/decrement product quantities
- **Total Calculation**: Automatic price calculations
- **Cart State**: Global state management with Zustand

### Product Catalog
- **Categories**: Mockups, graphic elements, design assets
- **File Types**: PSD, PNG, SVG support
- **Compatibility**: Photoshop, Figma, and other design tools
- **Pricing**: Individual product pricing
- **Designer Credits**: Attribution to original designers

### Animation System
- **GSAP Integration**: Professional-grade animations
- **Page Transitions**: Smooth navigation between pages
- **Scroll Animations**: Lenis-powered smooth scrolling
- **Text Animations**: Split-type for text effects
- **Custom Easing**: Custom animation curves

## 🎯 Performance Optimization

- **Next.js 15**: Latest performance optimizations
- **React 19**: Improved rendering performance
- **Image Optimization**: Next.js automatic image optimization
- **Code Splitting**: Automatic route-based code splitting
- **Static Generation**: Pre-rendered pages where possible

## 🔒 Security Considerations

- **Input Validation**: Client and server-side validation
- **XSS Protection**: React's built-in XSS protection
- **CSRF Protection**: Next.js built-in CSRF protection
- **Environment Variables**: Secure configuration management

## 🧪 Testing

```bash
# Run linting
pnpm lint

# Add testing framework (recommended)
pnpm add -D jest @testing-library/react @testing-library/jest-dom
```

## 📈 Monitoring and Analytics

Consider adding monitoring tools:

```bash
# Add analytics
pnpm add @vercel/analytics

# Add error tracking
pnpm add @sentry/nextjs
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and questions:

- **Documentation**: Check the [Next.js documentation](https://nextjs.org/docs)
- **Issues**: Create an issue in the repository
- **Community**: Join the Next.js community

## 🔄 Updates and Maintenance

### Regular Maintenance Tasks
- Update dependencies regularly
- Monitor for security vulnerabilities
- Update Next.js and React versions
- Optimize images and assets
- Review and update product catalog

### Performance Monitoring
- Monitor Core Web Vitals
- Track user engagement metrics
- Monitor cart abandonment rates
- Analyze page load times

---

**Format Archive** - Elevating digital design through curated assets and seamless experiences.
