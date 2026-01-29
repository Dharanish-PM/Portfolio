<template>
  <section id="hero" class="hero">
    <div class="hero-content">
      <div class="hero-text">
        <div class="title-line">
          <h1 class="name">Dharanish P M</h1>
          <h2 class="title">Software Engineer</h2>
        </div>
        <p class="subtitle">Java | Spring Boot | Microservices | Vue.js | AWS</p>
        <p class="tagline">Building scalable, microservices-based systems for production environments</p>
        <div class="cta-buttons">
          <a href="#experience" class="btn btn-primary">View Experience</a>
          <a href="/resume.pdf" class="btn btn-secondary" download>Download Resume</a>
        </div>
      </div>
      <div class="hero-visual">
        <div class="code-window">
          <div class="window-header">
            <span class="dot red"></span>
            <span class="dot yellow"></span>
            <span class="dot green"></span>
          </div>
          <div class="code-content">
            <pre><code><span class="keyword">class</span> <span class="class-name">Developer</span> {
  <span class="keyword">constructor</span>() {
    <span class="keyword">this</span>.name = <span class="string">"Full Stack Dev"</span>;
    <span class="keyword">this</span>.skills = [
      <span class="string">"Java"</span>, <span class="string">"Spring Boot"</span>,
      <span class="string">"Microservices"</span>, <span class="string">"Vue.js"</span>
    ];
    <span class="keyword">this</span>.passion = <span class="string">"Cloud Computing"</span>;
  }
}</code></pre>
          </div>
        </div>
      </div>
    </div>
    <div class="scroll-indicator">
      <span>Scroll Down</span>
      <div class="arrow">↓</div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero'
}
</script>

<style scoped>
.hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-top: 100px;
  position: relative;
}

.hero-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
  width: 100%;
}

.hero-text {
  animation: fadeInLeft 1s ease;
}

.title-line {
  display: flex;
  align-items: baseline;
  gap: 1.5rem;
  margin-bottom: 1.5rem;
  flex-wrap: wrap;
}

.name {
  font-size: 3.5rem;
  font-weight: 700;
  margin: 0;
  background: linear-gradient(135deg, var(--accent-blue), var(--accent-cyan));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  line-height: 1;
}

.title {
  font-size: 2rem;
  font-weight: 600;
  color: var(--text-primary);
  margin: 0;
  line-height: 1;
}

.subtitle {
  font-size: 1.2rem;
  color: var(--accent-cyan);
  margin-bottom: 1rem;
  font-weight: 500;
}

.tagline {
  font-size: 1.1rem;
  color: var(--text-secondary);
  margin-bottom: 2rem;
}

.cta-buttons {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

.hero-visual {
  animation: fadeInRight 1s ease;
}

.code-window {
  background: var(--bg-card);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 10px 30px var(--shadow);
}

.window-header {
  background: #1a1f35;
  padding: 12px 16px;
  display: flex;
  gap: 8px;
}

.dot {
  width: 12px;
  height: 12px;
  border-radius: 50%;
}

.dot.red { background: #ff5f56; }
.dot.yellow { background: #ffbd2e; }
.dot.green { background: #27c93f; }

.code-content {
  padding: 1.5rem;
  font-family: 'Courier New', monospace;
  font-size: 0.9rem;
  line-height: 1.6;
}

.keyword { color: #c678dd; }
.class-name { color: #e5c07b; }
.string { color: #98c379; }

.scroll-indicator {
  position: absolute;
  bottom: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 0.5rem;
  color: var(--text-secondary);
  animation: bounce 2s infinite;
}

.arrow {
  font-size: 1.5rem;
}

@keyframes fadeInLeft {
  from {
    opacity: 0;
    transform: translateX(-50px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fadeInRight {
  from {
    opacity: 0;
    transform: translateX(50px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes bounce {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(10px); }
}

@media (max-width: 768px) {
  .hero-content {
    grid-template-columns: 1fr;
    gap: 2rem;
  }

  .name {
    font-size: 2.5rem;
  }

  .title {
    font-size: 1.5rem;
  }

  .subtitle {
    font-size: 1rem;
  }

  .code-window {
    font-size: 0.8rem;
  }
}
</style>
