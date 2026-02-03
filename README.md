# Barney Gammond Website

A personal website built with [Craft CMS](https://craftcms.com/) and [Tailwind CSS](https://tailwindcss.com/).

## Overview

This is a modern, content-managed website powered by Craft CMS 5 with styling built using Tailwind CSS 4 and PostCSS.

## Requirements

- PHP 8.2+
- Node.js 18+
- Composer
- npm
- [DDEV](https://ddev.com/get-started/)

## Installation

### 1. Install PHP Dependencies

```bash
composer install
```

### 2. Install Node Dependencies

```bash
npm install
```

### 3. Set Up Environment
Run the following commands to import the ddev config, start the containers and install required packages.

```bash
ddev config

ddev start

ddev composer install
```

### 4. Initialize Craft CMS

```bash
ddev craft install
```
The .env will automatically be created with the necessary Craft values.

## Development

### Run the Dev Server

Start the development server with hot-reload for CSS:

```bash
npm start
```

This command runs Parcel to watch and compile your Tailwind CSS styles.

### Build for Production

```bash
npm run build
```

This creates optimized production builds of your CSS and assets.

## Project Structure

- **`config/`** - Craft CMS configuration files
- **`src/`** - Source CSS files (Tailwind CSS)
- **`templates/`** - Twig template files
- **`web/`** - Web-accessible assets and entry point
  - `web/dist/` - Compiled CSS and JS bundles (generated)
- **`storage/`** - Runtime data, caches, and logs
- **`vendor/`** - Composer dependencies

## Key Technologies

- **Craft CMS 5** - Headless/traditional CMS
- **Tailwind CSS 4** - Utility-first CSS framework
- **Parcel 2** - Web bundler for asset compilation
- **PostCSS** - CSS transformations
- **Twig** - Template engine

## Available Scripts

- `npm start` - Start development server with hot reload
- `npm run build` - Build for production

## License

ISC
