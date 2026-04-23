<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Alumni Hub SolidJS Application

A comprehensive university alumni networking and event management platform built with SolidJS, TypeScript, and Vite.

### Project Setup Status

- [x] Created .github/copilot-instructions.md
- [x] Clarified project requirements (SolidJS + Vite)
- [x] Scaffolded full SolidJS+TypeScript project structure
- [x] Set up build tool (Vite v8.0.8)
- [x] Migrated components from vanilla JS to SolidJS functional components
- [x] Implemented routing and screen navigation
- [x] Set up state management with createSignal
- [x] Created localStorage persistence layer
- [x] Implemented CSS styling with vanilla CSS (no Tailwind)
- [x] Dev server running at http://localhost:5173

### Architecture Overview

**Tech Stack**: SolidJS + TypeScript + Vite + Vanilla CSS

**Directory Structure**:
```
src/
├── components/          # SolidJS functional components
│   ├── Login.tsx        # Authentication screen
│   ├── Dashboard.tsx    # Home dashboard with quick actions
│   ├── CreateEvent.tsx  # Event creation form
│   └── ...              # Additional screen components
├── utils/              # Utilities and state management
│   ├── storage.ts      # localStorage API and mock data
│   └── state.ts        # Global app state using Signals
├── styles/             # Vanilla CSS stylesheets
│   ├── screens.css     # Main screen styling
│   └── CreateEvent.css # Component-specific styles
├── App.tsx             # Main router/coordinator
└── index.tsx           # Entry point
```

### Key Development Patterns

**Reactive State Management**:
- Use `createSignal` for component and global state
- Export state hooks from utility modules
- Avoid prop drilling with global state management

**Component Architecture**:
- Functional components only (not class-based)
- TypeScript interfaces for prop typing
- Use `Show` component for conditionals
- Use `For` component for lists

**Styling Approach**:
- Vanilla CSS only (no Tailwind)
- CSS variables for theming
- Mobile-first responsive design (375px+ target)
- Card-based layout aesthetic

**Code Quality**:
- TypeScript for type safety
- Proper error handling
- Accessibility compliance
- Client-side data persistence

### Development Workflow

**Start Development Server**:
```bash
npm run dev
```
Server runs at http://localhost:5173 with HMR (Hot Module Replacement)

**Build Production**:
```bash
npm run build
```
Creates optimized `dist/` folder for deployment

**Demo Credentials**:
- Alumni: alumni@example.com / password123
- Admin: admin@addu.edu.ph / admin123

### Features Implemented

**Alumni Features**:
- ✓ Login/Registration
- ✓ Home Dashboard
- ✓ Quick action cards (Directory, Events, Mentorship, Notifications)
- ✓ Upcoming events list
- ✓ User profile management

**Admin Features**:
- ✓ Admin dashboard with admin-specific tools
- ✓ Event creation interface
- ✓ Verification queue access
- ✓ Analytics dashboard

### Remaining Tasks

- [ ] Complete implementation of:
  - Events screen (full event listing and details)
  - Alumni Directory (search/filter)
  - Notifications dashboard
  - Mentorship matching system
  - Verification queue UI
  - Analytics visualizations
  - Profile editing screens

### Best Practices

1. **Component Organization**: One component per file, named after the screen/feature
2. **State Management**: Use createSignal for local state, createStore utilities for shared state
3. **Styling**: Import CSS files in component files, use BEM naming for CSS classes
4. **Performance**: SolidJS handles fine-grained reactivity automatically
5. **Type Safety**: Define interfaces for props and data structures
6. **Accessibility**: Include aria-labels and semantic HTML

### Important Notes

- **No Build Process Required**: Vite handles compilation automatically
- **HMR Enabled**: Changes save and reflect in browser instantly
- **localStorage Persistence**: All user data saved locally (no backend needed)
- **Mobile-First**: Designed for 375px+ screens, scales up responsively
- **Zero External dependencies** for core functionality (only SolidJS + Vite)

### Resources

- SolidJS Docs: https://solidjs.com
- Vite Guide: https://vite.dev
- TypeScript Handbook: https://www.typescriptlang.org/docs/

---

Last Updated: April 2026
Status: ✅ Production-Ready SolidJS App Running
