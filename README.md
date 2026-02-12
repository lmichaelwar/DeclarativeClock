# AllTime - Universal Time Widget

<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

A high-precision, monochrome clock widget featuring UTC as the dominant time display, along with POSIX, Binary, and Local time formats. Built as a Progressive Web App (PWA) for offline support and installation on any device.

## Features

- 🌍 **UTC Time Dominant** - The universal time standard takes center stage
- 🕰️ **Multiple Time Formats**:
  - UTC (Coordinated Universal Time) - Primary display with milliseconds
  - POSIX Timestamp - Unix epoch time
  - Binary Clock - Visual binary representation of UTC time
  - Local Time - Your timezone (less prominent by design)
- 📱 **Progressive Web App** - Install on any device, works offline
- ⚡ **Real-time Sync** - NIST time sync indicator
- 🎨 **Analog Clock** - Classic analog display showing local time
- 📐 **Responsive Design** - Works beautifully on desktop, tablet, and mobile
- 🌙 **Dark Theme** - Easy on the eyes in any lighting condition

## Live Demo

Visit the live app: [https://lmichaelwar.github.io/AllTime/](https://lmichaelwar.github.io/AllTime/)

## Screenshots

**Desktop:**
![Desktop View](https://github.com/user-attachments/assets/c68916c7-9824-4e12-b6c7-b2c2a6610c70)

**Mobile:**
![Mobile View](https://github.com/user-attachments/assets/c64e0592-b8a0-4ca7-a7dc-b64c95091f7f)

## Run Locally

**Prerequisites:** Node.js (v18 or higher recommended)

1. Clone the repository:
   ```bash
   git clone https://github.com/lmichaelwar/AllTime.git
   cd AllTime
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open your browser to `http://localhost:3000`

## Build for Production

Build the app for production deployment:

```bash
npm run build
```

The built files will be in the `dist/` directory.

Preview the production build locally:

```bash
npm run preview
```

## Deploy to GitHub Pages

This repository is configured to automatically deploy to GitHub Pages when you push to the `main` branch.

### Setup GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" in the left sidebar
3. Under "Build and deployment":
   - Source: Select "GitHub Actions"
4. Push to the `main` branch and the workflow will automatically build and deploy

The site will be available at: `https://<username>.github.io/AllTime/`

## PWA Features

AllTime is a Progressive Web App with:

- 📲 **Installable** - Add to home screen on any device
- 🔌 **Offline Support** - Works without internet connection via service worker
- ⚡ **Fast Loading** - Cached resources for instant load times
- 🎯 **Standalone Mode** - Runs like a native app

### Installing as PWA

**On Desktop (Chrome/Edge):**
1. Visit the site
2. Click the install icon in the address bar
3. Click "Install"

**On Mobile (iOS Safari):**
1. Visit the site
2. Tap the Share button
3. Scroll down and tap "Add to Home Screen"

**On Mobile (Android Chrome):**
1. Visit the site
2. Tap the menu (⋮)
3. Tap "Install app" or "Add to Home Screen"

## Technology Stack

- **React 19** - UI framework
- **TypeScript** - Type safety
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling
- **Lucide React** - Icons
- **Service Workers** - Offline support

## Project Structure

```
AllTime/
├── components/          # React components
│   ├── AnalogClock.tsx # Analog clock face
│   ├── BinaryClock.tsx # Binary time display
│   └── InfoPanel.tsx   # Digital time displays
├── hooks/              # Custom React hooks
│   └── usePreciseTime.ts # High-precision time updates
├── public/             # Static assets
│   ├── manifest.json   # PWA manifest
│   ├── service-worker.js # Service worker for offline support
│   └── *.png          # App icons
├── App.tsx            # Main app component
├── index.tsx          # App entry point
└── index.css          # Global styles

```

## Keyboard Shortcuts

- **Space** - Toggle minimal mode
- **Escape** - Reset view
- **Ctrl+M** - Toggle fullscreen

## Time Format Philosophy

Following the principle that "UTC should be the dominant time," this app prioritizes universal time standards:

1. **UTC** - The primary, most privileged time display
2. **POSIX & Binary** - Co-equal "ultimate times" representing universal standards
3. **Local Time** - Present but less prominent, acknowledging local context

The analog clock displays local time, maintaining the connection between the universal digital times and your local context.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

## Acknowledgments

- Built with [AI Studio](https://ai.studio/apps/drive/1O2aiU9dmeRpDSmnRDHdMQto8zX3z59ol)
- Time synchronization concept inspired by NIST time servers
