---
description: Repository Information Overview
alwaysApply: true
---

# Video App Candidate Assessment Information

## Summary
A sophisticated video creation and editing web application built with React. The project integrates advanced media processing capabilities using FFmpeg, PixiJS, and Fabric.js, and leverages various cloud services including Firebase, AWS, and Clerk for authentication and storage.

## Structure
- **src/**: Main application source code.
  - **components/**: Extensive collection of UI components for video editing and AI tools.
  - **pages/**: Application pages, dominated by the complex `VideoCreationPage`.
  - **redux/** & **mobx/**: State management logic using both Redux Toolkit and MobX.
  - **services/**: API wrappers for AWS, Google Drive, and other external services.
  - **utils/**: Utility functions for audio processing, canvas manipulation, and file handling.
- **public/**: Static assets and the main HTML entry point.
- **.zencoder/workflows/**: Configuration for Zencoder workflows.

## Language & Runtime
**Language**: JavaScript (React)  
**Version**: React 18.1.0  
**Build System**: Create React App (react-scripts 5.0.1)  
**Package Manager**: npm (implied by package-lock.json)

## Dependencies
**Main Dependencies**:
- **State Management**: `@reduxjs/toolkit`, `mobx`, `mobx-react`
- **Media Processing**: `@ffmpeg/ffmpeg`, `pixi.js`, `fabric`, `wavesurfer.js`
- **Authentication**: `@clerk/clerk-react`, `passport`
- **Cloud & Backend**: `firebase`, `aws-sdk`, `mongodb`, `express`
- **UI & Animation**: `animejs`, `sass`, `react-icons`, `lottie-react`

**Development Dependencies**:
- **Documentation**: `storybook`
- **Testing**: `@playwright/test`
- **Utilities**: `cross-env`, `tsx`, `webpack`

## Build & Installation
```bash
# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm run build
```

## Testing

**Framework**: Playwright & Jest (via react-scripts)
**Test Location**: Naming convention suggests `*.test.js` or `*.spec.js`, though primarily integrated with Playwright.
**Run Command**:
```bash
# Run Playwright tests
npm test

# Run tests in CI mode
npm run test:ci
```

## Storybook

**Run Command**:
```bash
npm run storybook
```
**Build Command**:
```bash
npm run build-storybook
```

## Main Files & Resources
- **Entry Point**: `src/index.js`
- **Main App Component**: `src/App.jsx`
- **Core Feature Page**: `src/pages/VideoCreationPage/VideoCreationPage.jsx`
- **Configuration**: `package.json`, `jsconfig.json`, `.eslintrc.js`
