# Psychology |Telehealth PA Directory Website

![Project Banner](assets/images/banner.png)

A comprehensive directory website showcasing telehealth psychology services across Pennsylvania.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support & Resources](#support--resources)

## Overview

Psychology |Telehealth PA is a directory website designed to connect patients with telehealth psychology providers in Pennsylvania. The site features a responsive 3-column grid layout, advanced filtering options, and detailed provider profiles.

## Features

- Responsive 3-column grid layout
- Advanced search and filtering
- Provider profiles with detailed information
- Category-based navigation
- Mobile-friendly design
- SEO optimized structure
- Contact forms for providers
- Interactive map integration

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/telehealth-pa.git

# Navigate to project directory
cd telehealth-pa

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
telehealth-pa/
├── assets/
│   ├── css/
│   ├── images/
│   └── js/
├── components/
│   ├── Directory/
│   ├── Header/
│   └── Footer/
├── data/
│   └── providers.json
├── pages/
├── public/
└── styles/
```

## Customization Guide

### Adding Directory Items

1. Navigate to `data/providers.json`
2. Add new provider entry:

```json
{
  "id": "unique-id",
  "name": "Provider Name",
  "specialty": "Clinical Psychology",
  "location": "Pittsburgh, PA",
  "telehealth": true,
  "contact": {
    "phone": "555-555-5555",
    "email": "provider@example.com"
  }
}
```

### Modifying Category Labels

1. Open `components/Directory/Categories.js`
2. Update category array:

```javascript
const categories = [
  "Clinical Psychology",
  "Behavioral Health",
  "Counseling",
  "Psychiatry"
];
```

### Updating Hero Section

1. Locate `components/Header/Hero.js`
2. Modify content:

```javascript
<div className="hero">
  <h1>Your New Heading</h1>
  <p>Your new description text</p>
</div>
```

### Customizing Colors

1. Navigate to `styles/variables.scss`
2. Update color variables:

```scss
$primary-color: #4A90E2;
$secondary-color: #2C3E50;
$accent-color: #E74C3C;
```

## Deployment

### Build for Production

```bash
# Generate production build
npm run build

# Test production build locally
npm run start
```

### Deploy to Hosting

1. Push to GitHub repository
2. Connect to hosting platform (Vercel/Netlify)
3. Configure build settings:
   - Build command: `npm run build`
   - Output directory: `out`

## Custom Domain Setup

1. Purchase domain name
2. Add DNS records:
   ```
   A Record: @ → Your-Server-IP
   CNAME: www → your-site.netlify.app
   ```
3. Configure SSL certificate
4. Update site settings in hosting platform

## Troubleshooting

### Common Issues

1. **Build Errors**
   - Clear cache: `npm run clean`
   - Delete node_modules: `rm -rf node_modules`
   - Reinstall dependencies: `npm install`

2. **Style Issues**
   - Clear browser cache
   - Check CSS specificity
   - Verify SCSS compilation

3. **Data Not Updating**
   - Verify JSON format
   - Clear local storage
   - Check API endpoints

## Support & Resources

- [Documentation Wiki](https://github.com/yourusername/telehealth-pa/wiki)
- [Issue Tracker](https://github.com/yourusername/telehealth-pa/issues)
- [Contributing Guidelines](CONTRIBUTING.md)

### Contact Support

- Email: support@telehealthpa.com
- Twitter: [@telehealthPA](https://twitter.com/telehealthPA)
- Discord: [Join our community](https://discord.gg/telehealthpa)

---

© 2024 Psychology |Telehealth PA. All rights reserved.