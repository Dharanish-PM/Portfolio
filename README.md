# Full Stack Developer Portfolio

A modern, professional portfolio website built with Vue.js showcasing 2 years of Full Stack development experience specializing in Java, Spring Boot, Microservices, and Cloud Computing.

## 🎨 Features

- **Modern Design**: Clean, professional dark mode with gradient accents
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Smooth Animations**: Engaging hover effects and scroll-based reveals
- **SEO-Friendly**: Semantic HTML structure for better search engine visibility
- **Performance Optimized**: Fast loading and efficient rendering

## 📋 Sections

1. **Hero Section** - Eye-catching introduction with call-to-action buttons
2. **About Me** - Professional background and expertise highlights
3. **Technical Skills** - Categorized skill showcase (Backend, Frontend, Cloud, etc.)
4. **Projects** - Detailed case studies with metrics and impact
5. **Experience** - Professional timeline with responsibilities
6. **Education** - Academic background and current learning
7. **Contact** - Multiple contact methods and message form

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Navigate to the project directory:
```bash
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

4. Open your browser and visit `http://localhost:5173`

## 🛠️ Build for Production

```bash
npm run build
```

The production-ready files will be in the `dist` directory.

## 📝 Customization

### Update Personal Information

1. **Hero Section** (`src/components/Hero.vue`):
   - Update your name in the `<h1>` tag
   - Modify the tagline and subtitle

2. **About Section** (`src/components/About.vue`):
   - Customize your professional summary
   - Update highlight items with your achievements

3. **Projects** (`src/components/Projects.vue`):
   - Replace with your actual projects
   - Update tech stacks, problems, solutions, and metrics

4. **Experience** (`src/components/Experience.vue`):
   - Add your work experience details
   - Update company names, dates, and responsibilities

5. **Education** (`src/components/Education.vue`):
   - Update university names and degrees
   - Modify graduation dates and CGPA

6. **Contact** (`src/components/Contact.vue` and `src/components/Footer.vue`):
   - Replace placeholder email with your actual email
   - Update GitHub and LinkedIn URLs
   - Modify location information

### Color Scheme

Edit CSS variables in `src/App.vue`:

```css
:root {
  --bg-primary: #0f172a;
  --bg-secondary: #1e293b;
  --accent-blue: #3b82f6;
  --accent-cyan: #06b6d4;
  --accent-purple: #8b5cf6;
}
```

### Add Resume

Place your resume PDF in the `public` folder as `resume.pdf` for the download button to work.

## 📦 Project Structure

```
portfolio/
├── public/              # Static assets
├── src/
│   ├── components/      # Vue components
│   │   ├── Header.vue
│   │   ├── Hero.vue
│   │   ├── About.vue
│   │   ├── Skills.vue
│   │   ├── Projects.vue
│   │   ├── Experience.vue
│   │   ├── Education.vue
│   │   ├── Contact.vue
│   │   └── Footer.vue
│   ├── App.vue         # Main app component
│   └── main.js         # App entry point
├── index.html
└── package.json
```

## 🌐 Deployment

### Deploy to Netlify

1. Build the project: `npm run build`
2. Drag and drop the `dist` folder to Netlify
3. Or connect your GitHub repository for automatic deployments

### Deploy to Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow the prompts

### Deploy to GitHub Pages

1. Update `vite.config.js` with your repository name
2. Run: `npm run build`
3. Push the `dist` folder to `gh-pages` branch

## 🎯 Tech Stack

- **Vue.js 3** - Progressive JavaScript framework
- **Vite** - Next-generation frontend tooling
- **CSS3** - Modern styling with gradients and animations
- **Google Fonts** - Inter font family

## 📄 License

This project is open source and available for personal use.

## 🤝 Contributing

Feel free to fork this project and customize it for your own portfolio!

## 📧 Contact

For questions or feedback, reach out via the contact form on the website.

---

**Built with ❤️ using Vue.js**
