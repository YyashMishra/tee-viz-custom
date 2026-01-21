# 🎨 Tee-Viz Custom - 3D T-Shirt Customizer

A modern, interactive web application that allows users to design and customize t-shirts in real-time using 3D visualization. Built with React, Three.js, and TypeScript.

![Version](https://img.shields.io/badge/version-0.0.0-blue.svg)
![React](https://img.shields.io/badge/React-18.3.1-61DAFB?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.5.3-3178C6?logo=typescript)
![Three.js](https://img.shields.io/badge/Three.js-0.161.0-000000?logo=three.js)
![Vite](https://img.shields.io/badge/Vite-5.4.1-646CFF?logo=vite)

## 📋 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Usage](#-usage)
- [Development](#-development)
- [Build & Deployment](#-build--deployment)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Features

### 🎯 Core Features
- **3D T-Shirt Visualization** - Interactive 3D model with real-time rendering
- **Color Customization** - Choose from 8 preset colors or pick a custom color
- **Image Upload** - Upload logos/designs (PNG/JPG, max 2MB)
- **Interactive Controls** - Rotate, zoom, and pan the 3D model
- **Real-time Preview** - See your design changes instantly
- **Drag & Drop** - Convenient file upload with drag-and-drop support
- **Responsive Design** - Works seamlessly on desktop and mobile devices
- **Toast Notifications** - User-friendly feedback for all actions

### 🎨 Design Features
- Modern glassmorphism UI
- Smooth animations and transitions
- Professional gradient backgrounds
- Intuitive user interface
- Accessible components (ARIA compliant)

## 🛠 Tech Stack

### Frontend Framework
- **React 18.3.1** - UI library with hooks
- **TypeScript 5.5.3** - Type-safe JavaScript
- **Vite 5.4.1** - Fast build tool and dev server

### 3D Graphics
- **Three.js 0.161.0** - 3D graphics library
- **@react-three/fiber 8.18.0** - React renderer for Three.js
- **@react-three/drei 9.122.0** - Useful helpers for R3F

### Routing & State
- **React Router DOM 6.26.2** - Client-side routing
- **TanStack Query 5.56.2** - Server state management

### UI Components
- **Radix UI** - Accessible component primitives
- **shadcn/ui** - Re-usable component library
- **Tailwind CSS 3.4.11** - Utility-first CSS framework
- **Lucide React** - Beautiful icon library
- **Sonner** - Toast notifications

### Form Handling
- **React Hook Form 7.53.0** - Form state management
- **Zod 3.23.8** - Schema validation

### Additional Libraries
- **date-fns 3.6.0** - Date manipulation
- **embla-carousel-react 8.3.0** - Carousel component
- **recharts 2.12.7** - Charting library
- **cmdk 1.0.0** - Command palette

## 📁 Project Structure

```
tee-viz-custom/
├── public/                      # Static assets
│   ├── robots.txt              # SEO robots file
│   └── model/                  # 3D model files (GLB/GLTF)
├── src/
│   ├── components/             # React components
│   │   ├── ColorPicker.tsx    # Color selection component
│   │   ├── FileUploader.tsx   # File upload with drag-drop
│   │   ├── Loader.tsx         # Loading spinner
│   │   ├── Navbar.tsx         # Navigation bar
│   │   ├── TShirtViewer.tsx   # 3D T-shirt renderer
│   │   └── ui/                # shadcn/ui components
│   │       ├── button.tsx
│   │       ├── card.tsx
│   │       ├── input.tsx
│   │       └── ...            # 40+ UI components
│   ├── hooks/                  # Custom React hooks
│   │   ├── use-mobile.tsx     # Mobile detection
│   │   └── use-toast.ts       # Toast notifications
│   ├── lib/
│   │   └── utils.ts           # Utility functions
│   ├── pages/                  # Route pages
│   │   ├── Home.tsx           # Landing page
│   │   ├── Customize.tsx      # T-shirt customizer
│   │   ├── Index.tsx          # Entry page
│   │   └── NotFound.tsx       # 404 page
│   ├── App.tsx                 # Main app component
│   ├── main.tsx               # App entry point
│   ├── index.css              # Global styles
│   └── App.css                # App-specific styles
├── .gitignore                  # Git ignore rules
├── components.json             # shadcn/ui config
├── eslint.config.js           # ESLint configuration
├── index.html                 # HTML entry point
├── package.json               # Dependencies
├── postcss.config.js          # PostCSS config
├── tailwind.config.ts         # Tailwind configuration
├── tsconfig.json              # TypeScript config
├── tsconfig.app.json          # App TS config
├── tsconfig.node.json         # Node TS config
├── vite.config.ts             # Vite configuration
└── README.md                  # This file
```

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
- **Node.js** >= 16.0.0 ([Download](https://nodejs.org/))
- **npm** >= 8.0.0 or **yarn** >= 1.22.0 or **bun** >= 1.0.0

### Installation

1. **Clone the repository**
```bash
git clone <YOUR_GIT_URL>
cd tee-viz-custom
```

2. **Install dependencies**

Using npm:
```bash
npm install
```

Using yarn:
```bash
yarn install
```

Using bun:
```bash
bun install
```

3. **Start the development server**

Using npm:
```bash
npm run dev
```

Using yarn:
```bash
yarn dev
```

Using bun:
```bash
bun dev
```

4. **Open your browser**

Navigate to [http://localhost:5173](http://localhost:5173) (or the port shown in your terminal)

## 💡 Usage

### Home Page
- Landing page with feature highlights
- "Start Customizing" CTA button
- Overview of how the customizer works

### Customize Page
The customization interface consists of:

1. **Color Picker Section**
   - 8 preset colors (Purple, Blue, Pink, Green, Yellow, Red, Black, White)
   - Custom color picker for unlimited color options
   - Real-time color preview on 3D model

2. **File Upload Section**
   - Drag-and-drop zone for easy uploads
   - Click to browse file system
   - Supports PNG and JPG formats (max 2MB)
   - Image preview after upload
   - Design appears on the front of the t-shirt

3. **3D Viewer**
   - Interactive 3D t-shirt model
   - Mouse controls:
     - Left click + drag: Rotate
     - Scroll: Zoom in/out
     - Right click + drag: Pan
   - Auto-rotation animation
   - Real-time design rendering

## 🔧 Development

### Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with HMR |
| `npm run build` | Build for production |
| `npm run build:dev` | Build in development mode |
| `npm run preview` | Preview production build locally |
| `npm run lint` | Run ESLint for code quality |

### Adding New Components

1. **UI Components** (shadcn/ui)
```bash
npx shadcn-ui@latest add [component-name]
```

2. **Custom Components**
Create new components in `src/components/` following the existing patterns:
```typescript
// src/components/MyComponent.tsx
import { FC } from 'react';

interface MyComponentProps {
  // Define props
}

const MyComponent: FC<MyComponentProps> = ({ /* props */ }) => {
  return (
    // Component JSX
  );
};

export default MyComponent;
```

### Code Style

- **TypeScript** - Strongly typed code
- **ESLint** - Code linting and formatting
- **Functional Components** - Use React hooks
- **CSS** - Tailwind utility classes

### Key Configuration Files

- `vite.config.ts` - Vite build configuration
- `tailwind.config.ts` - Tailwind CSS customization
- `tsconfig.json` - TypeScript compiler options
- `eslint.config.js` - Linting rules
- `components.json` - shadcn/ui settings

## 🏗 Build & Deployment

### Production Build

```bash
npm run build
```

This creates an optimized production build in the `dist/` directory.

### Preview Production Build

```bash
npm run preview
```

Test the production build locally before deployment.

### Deployment Options

#### Option 1: Vercel (Recommended)
```bash
npm install -g vercel
vercel
```

#### Option 2: Netlify
```bash
npm install -g netlify-cli
netlify deploy --prod
```

#### Option 3: GitHub Pages
Add to `package.json`:
```json
{
  "scripts": {
    "deploy": "vite build && gh-pages -d dist"
  }
}
```

#### Option 4: Static Hosting
Upload the `dist/` folder to any static hosting service:
- AWS S3 + CloudFront
- Firebase Hosting
- Cloudflare Pages
- DigitalOcean App Platform

### Environment Variables

Create a `.env` file for environment-specific variables:
```env
VITE_API_URL=your_api_url
VITE_APP_NAME=Tee-Viz Custom
```

Access in code:
```typescript
const apiUrl = import.meta.env.VITE_API_URL;
```

## 🎯 Project Architecture

### Component Hierarchy

```
App
├── BrowserRouter
│   ├── Home
│   │   ├── Navbar
│   │   └── Features Section
│   ├── Customize
│   │   ├── Navbar
│   │   ├── ColorPicker
│   │   ├── FileUploader
│   │   └── TShirtViewer (Canvas)
│   │       └── TShirtModel (3D)
│   └── NotFound
└── UI Providers (Toast, Tooltip, Query)
```

### State Management

- **Component State** - `useState` for local state
- **Server State** - TanStack Query for API data
- **Routing State** - React Router for navigation
- **Form State** - React Hook Form for forms

### 3D Rendering Flow

1. `TShirtViewer` component initializes Three.js canvas
2. `TShirtModel` creates 3D geometry
3. Texture loader processes uploaded images
4. Real-time material updates for color changes
5. OrbitControls enable user interaction
6. Animation loop updates rotation

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Contribution Guidelines

- Follow existing code style
- Add TypeScript types for all new code
- Test on multiple browsers
- Update documentation as needed
- Write meaningful commit messages

## 🐛 Known Issues & Limitations

- Currently uses a placeholder 3D model (box geometry)
- Texture positioning may need adjustment for different models
- File size limit is 2MB for uploaded designs
- 3D model performance may vary on older devices

## 🔮 Future Enhancements

- [ ] Upload custom 3D models (GLB/GLTF)
- [ ] Multiple design placement (front, back, sleeves)
- [ ] Design scaling and positioning controls
- [ ] Save/export designs
- [ ] Share designs via URL
- [ ] Print-ready file generation
- [ ] Shopping cart integration
- [ ] User accounts and saved designs
- [ ] More clothing items (hoodies, hats, etc.)
- [ ] Advanced texture effects (embroidery, print styles)

## 📄 License

This project is open source and available under the MIT License.

## 👤 Authors

**Mishra ji's Team**
- GitHub: [@mishrajiteam](https://github.com/mishrajiteam)

## 🙏 Acknowledgments

- [Lovable](https://lovable.dev) - Initial project setup
- [shadcn/ui](https://ui.shadcn.com/) - UI components
- [Three.js](https://threejs.org/) - 3D graphics
- [React Three Fiber](https://docs.pmnd.rs/react-three-fiber) - React renderer for Three.js
- [Radix UI](https://www.radix-ui.com/) - Accessible components

## 📞 Support

For support, email support@example.com or open an issue in the repository.

## 🔗 Links

- **Live Demo**: [Coming Soon]
- **Documentation**: This README
- **Bug Reports**: [GitHub Issues](https://github.com/yourusername/tee-viz-custom/issues)
- **Feature Requests**: [GitHub Discussions](https://github.com/yourusername/tee-viz-custom/discussions)

---

Made with ❤️ by Mishra ji's Team
