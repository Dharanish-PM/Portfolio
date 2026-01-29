# Portfolio Customization Guide

This guide will help you personalize your portfolio with your own information.

## 🎯 Quick Start Checklist

- [ ] Update name and title in Hero section
- [ ] Replace email, GitHub, and LinkedIn links
- [ ] Add your projects with real data
- [ ] Update work experience details
- [ ] Modify education information
- [ ] Add your resume PDF
- [ ] Customize color scheme (optional)
- [ ] Add your profile photo (optional)

## 📝 Step-by-Step Customization

### 1. Hero Section (`src/components/Hero.vue`)

**Line 5**: Update your name
```vue
<h1 class="name">Your Name</h1>
<!-- Change to -->
<h1 class="name">John Doe</h1>
```

**Line 7**: Modify subtitle if needed
```vue
<p class="subtitle">Java | Spring Boot | Microservices | Vue.js | Cloud</p>
```

**Line 8**: Update tagline
```vue
<p class="tagline">Building scalable, high-performance web applications</p>
```

### 2. About Section (`src/components/About.vue`)

**Lines 20-24**: Update your professional intro
```vue
<p class="intro">
  Full Stack Developer with <strong>2 years of experience</strong>...
</p>
```

**Lines 26-48**: Customize highlight items with your achievements

### 3. Skills Section (`src/components/Skills.vue`)

**Lines 6-70**: Update skill categories and tags to match your expertise

Add or remove skills:
```vue
<span class="tag">Your Skill</span>
```

### 4. Projects Section (`src/components/Projects.vue`)

Replace each project card (lines 5-150) with your actual projects:

```vue
<div class="project-card card">
  <div class="project-header">
    <h3>Your Project Name</h3>
    <div class="project-tags">
      <span class="tech-tag">Tech 1</span>
      <span class="tech-tag">Tech 2</span>
    </div>
  </div>
  <div class="project-content">
    <div class="project-section">
      <h4>🎯 Problem</h4>
      <p>Describe the problem you solved</p>
    </div>
    <div class="project-section">
      <h4>💡 Solution</h4>
      <p>Explain your solution</p>
    </div>
    <div class="project-section">
      <h4>📈 Impact</h4>
      <ul>
        <li>Key achievement 1</li>
        <li>Key achievement 2</li>
      </ul>
    </div>
  </div>
  <div class="project-metrics">
    <div class="metric">
      <span class="metric-value">50%</span>
      <span class="metric-label">Improvement</span>
    </div>
  </div>
</div>
```

### 5. Experience Section (`src/components/Experience.vue`)

**Lines 6-50**: Update work experience

```vue
<div class="timeline-item">
  <div class="timeline-marker"></div>
  <div class="timeline-content card">
    <div class="timeline-header">
      <div>
        <h3>Your Job Title</h3>
        <h4>Company Name</h4>
      </div>
      <span class="timeline-date">Start - End Date</span>
    </div>
    <ul class="responsibilities">
      <li>Responsibility 1</li>
      <li>Responsibility 2</li>
    </ul>
    <div class="tech-stack">
      <span class="tech">Technology</span>
    </div>
  </div>
</div>
```

### 6. Education Section (`src/components/Education.vue`)

**Lines 6-25**: Update Master's degree info
```vue
<h3>MSc in Cloud Computing</h3>
<h4>National College of Ireland</h4>
<p class="duration">Expected Graduation: January 2027</p>
```

**Lines 27-48**: Update Bachelor's degree info
```vue
<h3>B.E. Computer Science and Engineering</h3>
<h4>University Name</h4>
<p class="cgpa">CGPA: <strong>8.90 / 10.0</strong></p>
```

**Lines 52-75**: Update "Currently Learning" section

### 7. Contact Section (`src/components/Contact.vue`)

**Line 5**: Update intro message
```vue
<p class="contact-intro">
  I'm currently open to Summer Internship and Software Engineering roles.
</p>
```

**Lines 12-14**: Update email
```vue
<a href="mailto:your.email@example.com" class="info-item">
  ...
  <p>your.email@example.com</p>
</a>
```

**Lines 16-22**: Update GitHub URL
```vue
<a href="https://github.com/yourusername" target="_blank" class="info-item">
  ...
  <p>github.com/yourusername</p>
</a>
```

**Lines 24-30**: Update LinkedIn URL
```vue
<a href="https://linkedin.com/in/yourusername" target="_blank" class="info-item">
  ...
  <p>linkedin.com/in/yourusername</p>
</a>
```

**Lines 32-38**: Update location
```vue
<div class="info-item">
  ...
  <p>Ireland</p>
</div>
```

### 8. Footer Section (`src/components/Footer.vue`)

**Lines 5-7**: Update footer description
```vue
<h3>&lt;Dev/&gt;</h3>
<p>Full Stack Web Developer specializing in...</p>
```

**Lines 24-26**: Update GitHub link
```vue
<a href="https://github.com/yourusername" target="_blank">
```

**Lines 30-32**: Update LinkedIn link
```vue
<a href="https://linkedin.com/in/yourusername" target="_blank">
```

**Lines 36-38**: Update email link
```vue
<a href="mailto:your.email@example.com">
```

**Line 46**: Update copyright name
```vue
<p>&copy; {{ currentYear }} Your Name. Built with Vue.js</p>
```

## 🎨 Optional Customizations

### Add Profile Photo

Replace the placeholder in `src/components/About.vue` (lines 6-14):

```vue
<div class="about-image">
  <img src="/path-to-your-photo.jpg" alt="Your Name" class="profile-photo" />
</div>
```

Add this CSS:
```css
.profile-photo {
  width: 100%;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(59, 130, 246, 0.3);
}
```

### Change Color Scheme

Edit `src/App.vue` (lines 45-52):

```css
:root {
  --bg-primary: #0f172a;        /* Main background */
  --bg-secondary: #1e293b;      /* Secondary background */
  --bg-card: #1e293b;           /* Card background */
  --text-primary: #f1f5f9;      /* Main text color */
  --text-secondary: #cbd5e1;    /* Secondary text */
  --accent-blue: #3b82f6;       /* Primary accent */
  --accent-cyan: #06b6d4;       /* Secondary accent */
  --accent-purple: #8b5cf6;     /* Tertiary accent */
}
```

### Add Resume Download

1. Place your resume PDF in the `public` folder
2. Name it `resume.pdf`
3. The download button in Hero section will automatically work

### Customize Fonts

Change the font in `src/App.vue` (line 39):

```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

body {
  font-family: 'Poppins', sans-serif;
}
```

## 🔧 Form Integration

The contact form currently simulates submission. To make it functional:

### Option 1: Formspree

1. Sign up at [formspree.io](https://formspree.io)
2. Get your form endpoint
3. Update `src/components/Contact.vue`:

```vue
<form @submit.prevent="handleSubmit" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: Netlify Forms

1. Add `netlify` attribute to form:
```vue
<form name="contact" netlify @submit.prevent="handleSubmit">
```

### Option 3: EmailJS

1. Sign up at [emailjs.com](https://www.emailjs.com)
2. Install: `npm install @emailjs/browser`
3. Update the `handleSubmit` method with EmailJS integration

## ✅ Final Checklist

Before deploying:

- [ ] All personal information updated
- [ ] All links working (email, GitHub, LinkedIn)
- [ ] Resume PDF added to public folder
- [ ] Projects reflect your actual work
- [ ] Experience and education accurate
- [ ] Contact form tested
- [ ] Responsive design checked on mobile
- [ ] All placeholder text replaced
- [ ] SEO meta tags updated in `index.html`

## 🚀 Ready to Deploy!

Once customized, follow the deployment instructions in README.md to publish your portfolio online.
