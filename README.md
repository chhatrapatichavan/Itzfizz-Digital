# Itzfizz Landing Page

A modern, responsive landing page with smooth scroll-driven animations built with Next.js, Tailwind CSS, and GSAP.

## 🚀 Features

- **Modern Design**: Beautiful gradient backgrounds with glassmorphism effects
- **Smooth Animations**: GSAP-powered animations with 60fps performance
- **Scroll-Driven Interactions**: Car animation that responds to scroll position
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Premium UX**: Smooth transitions and micro-interactions

## 🛠️ Tech Stack

- **Framework**: Next.js 14
- **Styling**: Tailwind CSS
- **Animations**: GSAP with ScrollTrigger
- **Language**: JavaScript/JSX

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd itzfizz-landing-page
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🎯 Project Structure

```
itzfizz-landing-page/
├── components/
│   └── HeroSection.jsx          # Main hero component with animations
├── pages/
│   ├── _app.js                  # App wrapper with global styles
│   └── index.js                 # Home page
├── styles/
│   └── globals.css              # Global styles and Tailwind imports
├── public/                      # Static assets
├── package.json                 # Dependencies and scripts
├── tailwind.config.js           # Tailwind configuration
├── next.config.js               # Next.js configuration
└── README.md                    # This file
```

## 🎨 Animation Details

### Initial Load Animations
- **Headline**: Fades in and moves upward with easing
- **Statistics**: Staggered appearance with scale and fade effects
- **Background**: Animated gradient orbs with pulse effects

### Scroll-Driven Animations
- **Car Movement**: Horizontal movement across screen based on scroll progress
- **Parallax Effects**: Background elements move at different speeds
- **Smooth Scrubbing**: 1-second lag for natural scroll-based motion

### Performance Optimizations
- Uses `transform` properties for GPU acceleration
- `will-change` CSS property for optimized rendering
- Efficient ScrollTrigger cleanup to prevent memory leaks
- 60fps animations with optimized easing functions

## 🚀 Deployment

### Deploy to Vercel (Recommended)

1. **Push to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin <your-github-repo-url>
   git push -u origin main
   ```

2. **Deploy to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Vercel will automatically detect Next.js and deploy

### Deploy to GitHub Pages

1. **Install gh-pages**
   ```bash
   npm install --save-dev gh-pages
   ```

2. **Update package.json scripts**
   ```json
   {
     "scripts": {
       "export": "next build && next export",
       "deploy": "gh-pages -d out"
     }
   }
   ```

3. **Update next.config.js**
   ```javascript
   const nextConfig = {
     output: 'export',
     trailingSlash: true,
     images: {
       unoptimized: true
     }
   }
   ```

4. **Deploy**
   ```bash
   npm run export
   npm run deploy
   ```

## 🎮 Customization

### Modifying Colors
Edit the gradient classes in `HeroSection.jsx`:
```jsx
className="bg-gradient-to-br from-purple-900 via-blue-900 to-indigo-900"
```

### Adjusting Animations
Modify GSAP timelines in `HeroSection.jsx`:
```javascript
// Change animation duration
duration: 1.2,

// Adjust easing
ease: 'power3.out',

// Modify stagger delay
stagger: 0.2
```

### Adding New Sections
1. Create new components in `/components`
2. Import and use in `pages/index.js`
3. Add ScrollTrigger animations as needed

## 🔧 Development Commands

```bash
# Development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Lint code
npm run lint
```

## 📱 Responsive Breakpoints

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## 🌟 Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- iOS Safari 14+
- Android Chrome 90+

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

---

**Built with ❤️ using Next.js, Tailwind CSS, and GSAP**
