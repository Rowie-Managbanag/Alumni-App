# AdDU Alumni Hub - SolidJS Application

A comprehensive university alumni networking and event management platform built with **SolidJS**, **TypeScript**, and **Vite**.

## Features

### Alumni Features
- **Authentication**: Secure login and registration system
- **Home Dashboard**: Quick access to key features and upcoming events
- **Alumni Directory**: Search and connect with fellow graduates
- **Events Management**: Browse, register for, and track events
- **Mentorship Network**: Connect with mentors and mentees
- **Notifications**: Real-time updates on profile activities
- **AI Matching**: Intelligent alumni-job matching system
- **Calendar**: Personal event and activity calendar
- **User Profile**: Comprehensive alumni profile management

### Admin Features
- **Admin Dashboard**: System overview and management controls
- **Verification Queue**: Review and verify alumni profiles
- **Event Manager**: Create, edit, and manage alumni events
- **Analytics**: Detailed platform analytics and statistics
- **Invitation Builder**: Create and send alumni invitations

## Tech Stack

- **Framework**: SolidJS (v1.x) - Reactive JavaScript framework
- **Build Tool**: Vite v8.0.8 - Next-generation frontend tooling
- **Language**: TypeScript - Type-safe development
- **Styling**: Vanilla CSS - Custom styling with no dependencies
- **Storage**: localStorage - Client-side data persistence
- **Node**: v14+ required

## Project Structure

```
src/
├── components/          # SolidJS components for each screen
│   ├── Login.tsx        # Authentication screen
│   ├── Dashboard.tsx    # Home dashboard
│   ├── CreateEvent.tsx  # Event creation form
│   └── ...              # Additional screens
├── utils/              # Utility functions and state management
│   ├── storage.ts      # localStorage and data persistence
│   ├── state.ts        # Global app state using Signals
│   └── helpers.ts      # Common utility functions
├── styles/             # Vanilla CSS stylesheets
│   ├── screens.css     # All screen styling
│   └── CreateEvent.css # Component-specific styles
├── App.tsx             # Main app component with routing
├── index.tsx           # Entry point
└── vite.config.ts      # Vite configuration
```

## Getting Started

### Prerequisites
- Node.js v14 or higher
- npm, yarn, or pnpm package manager

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open [http://localhost:5173](http://localhost:5173) in your browser

### Demo Credentials

**Alumni Account:**
- Email: `alumni@example.com`
- Password: `password123`

**Admin Account:**
- Email: `admin@addu.edu.ph`
- Password: `admin123`

## Available Scripts

### Development
```bash
npm run dev     # Start dev server with HMR (Hot Module Replacement)
npm run preview # Preview production build locally
npm run build   # Build for production
```

### Build Output
```bash
dist/           # Production-ready files
├── index.html  # Minified HTML
├── assets/     # Bundled & optimized JS/CSS
└── ...         # Static files
```

## Key Technologies & Patterns

### SolidJS Reactivity
- **createSignal**: Reactive state management for component data
- **createEffect**: Automatic reactive dependencies
- **Show**: Conditional rendering with fine-grained reactivity
- **For**: Efficient list rendering

### State Management
- Global app state via `createAppState()` hook
- User authentication state tracking
- Event and notification state management
- localStorage persistence

### Component Architecture
- Functional components (not class-based)
- TypeScript interfaces for prop typing
- Vanilla CSS modules for styling
- Mobile-first responsive design (375px+ target)

## Styling

The application uses **vanilla CSS** with:
- CSS variables for theming (Navy `#1a2a6c`, Blue `#2563eb`)
- Mobile-first responsive design
- Card-based layout aesthetic
- Smooth transitions and hover effects
- Accessibility-first approach

### Color Palette
- **Navy**: `#1a2a6c` - Primary brand color
- **Blue**: `#2563eb` - Secondary accent color
- **Teal**: `#14b8a6` - Accent highlights
- **Gold**: `#f59e0b` - Admin actions

## API & Data

- **No external APIs** - Client-side only
- **localStorage** - Persistent data storage
- **Mock Data** - Seed data for demo purposes
- User sessions maintained across page refreshes

## Deployment

### Build for Production
```bash
npm run build
```

### Deploy to GitHub Pages
```bash
# Build the app
npm run build

# Deploy the dist/ folder to GitHub Pages
# See GitHub documentation for static site hosting
```

### Deploy to Other Platforms
The app can be deployed to:
- Vercel
- Netlify
- Firebase Hosting
- AWS Amplify
- Traditional web servers

The `dist/` folder contains all required production files (HTML, CSS, JS).

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari 14+, Chrome Android)

## Contributing

Development workflow:
1. Create feature branch
2. Make changes with HMR
3. Test in dev server
4. Build and verify production
5. Submit PR

## License

University Alumni Hub Project - Private

## Support

For questions or issues, contact the development team.

---

**Last Updated**: April 2026  
**Built with SolidJS** ⚡ **Powered by Vite** ⚙️
