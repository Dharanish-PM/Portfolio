<template>
  <section 
    id="about" 
    class="about"
    v-motion
    :initial="{ opacity: 0, y: 50 }"
    :visible="{ opacity: 1, y: 0, transition: { duration: 600, ease: 'easeOut' } }"
  >
    <h2>About Me</h2>
    <div class="about-content">
      <div class="about-image">
        <img src="/myimage.jpg" alt="Dharanish P M" class="profile-photo" />
      </div>
      <div class="about-text">
        <p class="intro">
          Full Stack Developer with <strong>2 years of experience</strong> building production-grade backend systems and cloud-ready web applications.
        </p>
        <div class="highlights">
          <div class="highlight-item">
            <span class="icon">🚀</span>
            <p>Strong backend expertise with <strong>Java Spring Boot</strong> and <strong>microservices</strong> architecture</p>
          </div>
          <div class="highlight-item">
            <span class="icon">💼</span>
            <p>Experience building <strong>revenue-critical, search-driven systems</strong> for e-commerce platforms</p>
          </div>
          <div class="highlight-item">
            <span class="icon">⚡</span>
            <p>Comfortable owning features <strong>end-to-end</strong>: design → development → deployment</p>
          </div>
          <div class="highlight-item">
            <span class="icon">☁️</span>
            <p>Currently pursuing <strong>MSc in Cloud Computing</strong> (graduating Jan 2027)</p>
          </div>
          <div class="highlight-item">
            <span class="icon">📍</span>
            <p>Visa Status | <strong>Stamp 2 Visa</strong>, with Part-time Work Eligibility</p>
          </div>
          <div class="highlight-item">
            <span class="icon">📍</span>
            <p>Based in <strong>Ireland</strong>, open to Summer Internship and Software Engineering roles</p>
          </div>
        
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style scoped>
.about {
  background: rgba(30, 41, 59, 0.3);
  border-radius: 20px;
  margin: 2rem auto;
}

.about-content {
  display: grid;
  grid-template-columns: 300px 1fr;
  gap: 3rem;
  align-items: start;
}

.about-image {
  position: sticky;
  top: 100px;
}

.profile-photo {
  width: 100%;
  aspect-ratio: 1;
  object-fit: cover;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(59, 130, 246, 0.3);
  border: 4px solid rgba(6, 182, 212, 0.2);
}

.image-placeholder {
  width: 100%;
  aspect-ratio: 1;
  background: linear-gradient(135deg, var(--accent-blue), var(--accent-cyan));
  border-radius: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 8rem;
  box-shadow: 0 10px 30px rgba(59, 130, 246, 0.3);
}

.image-placeholder svg {
  width: 60%;
  height: 60%;
}

.about-text {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.intro {
  font-size: 1.2rem;
  line-height: 1.8;
  color: var(--text-secondary);
}

.intro strong {
  color: var(--accent-cyan);
  font-weight: 600;
}

.highlights {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.highlight-item {
  display: flex;
  gap: 1rem;
  align-items: start;
  padding: 1.5rem;
  background: var(--bg-card);
  border-radius: 12px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.highlight-item:hover {
  transform: translateX(10px);
  box-shadow: 0 4px 12px var(--shadow);
}

.icon {
  font-size: 2rem;
  flex-shrink: 0;
}

.highlight-item p {
  color: var(--text-secondary);
  line-height: 1.6;
}

.highlight-item strong {
  color: var(--text-primary);
  font-weight: 600;
}

@media (max-width: 968px) {
  .about-content {
    grid-template-columns: 1fr;
    gap: 2rem;
  }

  .about-image {
    position: relative;
    top: 0;
    max-width: 250px;
    margin: 0 auto;
  }
}
</style>
