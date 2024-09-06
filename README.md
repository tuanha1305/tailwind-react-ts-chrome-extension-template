
# Tailwind React TypeScript Chrome Extension Template

A boilerplate for building Chrome extensions using **React**, **TypeScript**, and **Tailwind CSS**. This template includes Vite, Webpack, and necessary configurations to create scalable Chrome extensions with modern web technologies.

## Features

- **React 18** and **TypeScript** for building robust UIs.
- **Tailwind CSS** for easy styling.
- **Webpack** for bundling.
- Chrome extension setup with **content scripts**, **background scripts**, **popups**, and **options pages**.
- Support for **React Router** in the Chrome extension's new tab.

## Project Structure

```bash
├── src/
│   ├── assets/              # Tailwind CSS configuration
│   ├── background/          # Background scripts
│   ├── contentScript/       # Content scripts
│   ├── options/             # Options page
│   ├── popup/               # Popup script and UI
│   ├── tabs/                # Custom new tab page with React Router
├── dist/                    # Output directory after build
├── static/                  # Static assets such as icons and manifest.json
├── package.json             # Project dependencies and scripts
├── tailwind.config.js       # Tailwind CSS configuration
├── webpack.common.js        # Webpack shared configuration
├── webpack.dev.js           # Webpack development configuration
├── webpack.prod.js          # Webpack production configuration
└── tsconfig.json            # TypeScript configuration
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/tailwind-react-ts-chrome-extension-template.git
   ```

2. Install dependencies using `yarn` or `npm`:

   ```bash
   yarn install
   # or
   npm install
   ```

3. Start the development server:

   ```bash
   yarn watch
   # or
   npm run watch
   ```

4. Build for production:

   ```bash
   yarn build
   # or
   npm run build
   ```

## Usage

- **Popup**: Customize the extension popup in `src/popup`.
- **Options Page**: Customize the options page in `src/options`.
- **Background Script**: Write background logic in `src/background/background.ts`.
- **Content Script**: Inject custom logic into web pages via `src/contentScript/contentScript.ts`.
- **New Tab**: Build a custom new tab page in `src/tabs` with React Router.

## Chrome Extension Setup

1. Build the extension using the build command.
2. Open Chrome and navigate to `chrome://extensions`.
3. Enable **Developer mode**.
4. Click **Load unpacked** and select the `dist` folder from the project.

## License

This project is licensed under the **MIT License**.
