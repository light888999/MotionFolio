# David Noden - Portfolio Website

A modern, interactive portfolio website showcasing my work as a Full-Stack Engineer. Built with React, TypeScript, and Three.js, featuring smooth animations, 3D elements, and an interactive chess game.

## 🚀 Features

- **Interactive Landing Page** - Animated hero section with smooth scrolling
- **About Section** - Professional background and skills overview
- **Work Showcase** - Horizontal scrolling gallery of featured projects
- **Career Timeline** - Professional experience and achievements
- **Tech Stack** - Visual display of technologies and tools
- **Contact Section** - Easy ways to get in touch
- **Responsive Design** - Optimized for desktop, tablet, and mobile devices
- **Smooth Animations** - Powered by GSAP and Lenis smooth scroll
- **3D Elements** - Three.js integration for enhanced visuals

## 🛠️ Tech Stack

### Core
- **React 18** - UI library
- **TypeScript** - Type-safe JavaScript
- **Vite** - Build tool and dev server
- **React Router** - Client-side routing

### Animation & 3D
- **GSAP** - Advanced animations
- **Lenis** - Smooth scrolling
- **Three.js** - 3D graphics
- **@react-three/fiber** - React renderer for Three.js
- **@react-three/drei** - Useful helpers for react-three-fiber

### Styling
- **CSS3** - Custom styling with animations
- **React Icons** - Icon library

### Other Libraries
- **chess.js** - Chess game logic
- **stockfish.js** - Chess engine
- **@vercel/analytics** - Analytics integration

## 📦 Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd portfolio
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

The site will be available at `http://localhost:5173` (or the port shown in terminal).

## 🎯 Available Scripts

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build for production
- `npm run preview` - Preview production build locally
- `npm run lint` - Run ESLint

## 📁 Project Structure

```
portfolio/
├── public/
│   ├── images/          # Project images and assets
│   └── videos/          # Video files for projects
├── src/
│   ├── components/      # React components
│   │   ├── About.tsx
│   │   ├── Career.tsx
│   │   ├── Contact.tsx
│   │   ├── Landing.tsx
│   │   ├── Navbar.tsx
│   │   ├── Work.tsx
│   │   └── ...
│   ├── pages/           # Page components
│   │   ├── MyWorks.tsx
│   │   └── Play.tsx
│   ├── config.ts        # Portfolio data configuration
│   ├── main.tsx         # Entry point
│   └── App.tsx          # Main app component
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

## ⚙️ Configuration

All portfolio content is managed in `src/config.ts`. Update the following sections:

- **Developer Info** - Name, title, description
- **Social Links** - GitHub, LinkedIn, email, phone
- **About Section** - Personal description
- **Experiences** - Work history and roles
- **Projects** - Portfolio projects with images/videos
- **Skills** - Technical skills and tools
- **Contact** - Contact information

### Adding a Project

Add a new project object to `config.projects`:

```typescript
{
    id: 7,
    title: "Project Name",
    category: "Category",
    technologies: "Tech Stack",
    image: "/images/project.png",
    video: "/videos/project.mp4", // Optional
    description: "Project description"
}
```

### Adding a Video Instead of Image

Set the `video` property in the project config:

```typescript
{
    id: 1,
    title: "Guestboard",
    video: "/videos/guestboard.mp4",
    image: "/images/guestboard.png", // Used as poster
    // ...
}
```

## 🎨 Customization

### Colors & Styling
- Modify CSS files in `src/components/styles/`
- Global styles can be added to `src/index.css` or `src/App.css`

### Animations
- GSAP animations are configured in individual components
- Lenis smooth scroll settings are in `Navbar.tsx`

### 3D Elements
- Three.js scenes can be added in components using `@react-three/fiber`

## 🚀 Deployment

### Build for Production

```bash
npm run build
```

The `dist/` folder will contain the production-ready files.

### Deploy to Vercel

1. Push your code to GitHub
2. Import the repository in Vercel
3. Vercel will automatically detect Vite and configure the build

The site is configured for Vercel deployment with analytics integration.

## 📝 License

This project is private and proprietary.

## 👤 Author

**David Noden**
- Email: david.noden.dev@gmail.com
- GitHub: [@light888999](https://github.com/light888999)
- LinkedIn: [David Noden](https://www.linkedin.com/in/david-noden-6a53843a9/)
- Location: Leicester City, United Kingdom

## 🙏 Acknowledgments

- Built with modern web technologies
- Inspired by contemporary portfolio designs
- Uses open-source libraries and frameworks
