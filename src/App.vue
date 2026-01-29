<template>
  <div id="app">
    <Header />
    <Hero />
    <About />
    <Skills />
    <Experience />
    <Education />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Experience from './components/Experience.vue'
import Education from './components/Education.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    About,
    Skills,
    Experience,
    Education,
    Contact,
    Footer
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --bg-primary: #0f172a;
  --bg-secondary: #1e293b;
  --bg-card: #1e293b;
  --text-primary: #f1f5f9;
  --text-secondary: #cbd5e1;
  --accent-blue: #3b82f6;
  --accent-cyan: #06b6d4;
  --accent-purple: #8b5cf6;
  --shadow: rgba(0, 0, 0, 0.3);
}

body {
  font-family: 'Inter', sans-serif;
  background: linear-gradient(135deg, var(--bg-primary) 0%, #1a1f35 100%);
  color: var(--text-primary);
  line-height: 1.6;
  overflow-x: hidden;
}

#app {
  min-height: 100vh;
}

section {
  padding: 80px 20px;
  max-width: 1200px;
  margin: 0 auto;
}

h2 {
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: 3rem;
  text-align: center;
  background: linear-gradient(135deg, var(--accent-blue), var(--accent-cyan));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.card {
  background: var(--bg-card);
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 6px var(--shadow);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px var(--shadow);
}

.btn {
  display: inline-block;
  padding: 12px 32px;
  border-radius: 8px;
  font-weight: 600;
  text-decoration: none;
  transition: all 0.3s ease;
  cursor: pointer;
  border: none;
  font-size: 1rem;
}

.btn-primary {
  background: linear-gradient(135deg, var(--accent-blue), var(--accent-cyan));
  color: white;
}

.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 16px rgba(59, 130, 246, 0.3);
}

.btn-secondary {
  background: transparent;
  border: 2px solid var(--accent-blue);
  color: var(--accent-blue);
}

.btn-secondary:hover {
  background: var(--accent-blue);
  color: white;
}

@media (max-width: 768px) {
  section {
    padding: 60px 20px;
  }
  
  h2 {
    font-size: 2rem;
  }
}
</style>
