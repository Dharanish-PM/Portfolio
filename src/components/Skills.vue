<template>
  <section 
    id="skills" 
    class="skills"
    v-motion
    :initial="{ opacity: 0, y: 50 }"
    :visible="{ opacity: 1, y: 0, transition: { duration: 600, ease: 'easeOut' } }"
  >
    <h2>Technical Skills</h2>
    <div class="skills-grid">
      <div class="skill-category card">
        <div class="category-icon">⚙️</div>
        <h3>Backend</h3>
        <div class="skill-tags">
          <span class="tag">Java</span>
          <span class="tag">Spring Boot</span>
          <span class="tag">Spring MVC</span>
          <span class="tag">Spring Data JPA</span>
          <span class="tag">Hibernate</span>
        </div>
      </div>

      <div class="skill-category card">
        <div class="category-icon">🎨</div>
        <h3>Frontend</h3>
        <div class="skill-tags">
          <span class="tag">JavaScript</span>
          <span class="tag">Vue.js</span>
          <span class="tag">HTML</span>
          <span class="tag">CSS</span>
        </div>
      </div>

      <div class="skill-category card">
        <div class="category-icon">🏗️</div>
        <h3>Architecture</h3>
        <div class="skill-tags">
          <span class="tag">Microservices</span>
          <span class="tag">RESTful APIs</span>
          <span class="tag">Clean Architecture</span>
        </div>
      </div>

      <div class="skill-category card">
        <div class="category-icon">💾</div>
        <h3>Data & Search</h3>
        <div class="skill-tags">
          <span class="tag">MySQL</span>
          <span class="tag">MongoDB</span>
          <span class="tag">Apache Solr</span>
        </div>
      </div>

      <div class="skill-category card">
        <div class="category-icon">📡</div>
        <h3>Messaging & Caching</h3>
        <div class="skill-tags">
          <span class="tag">Apache Kafka</span>
          <span class="tag">Redis</span>
        </div>
      </div>

      <div class="skill-category card">
        <div class="category-icon">☁️</div>
        <h3>DevOps & Cloud</h3>
        <div class="skill-tags">
          <span class="tag">AWS</span>
          <span class="tag">Docker</span>
          <span class="tag">Jenkins</span>
          <span class="tag">CI/CD Pipelines</span>
          <span class="tag">Git</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Skills'
}
</script>

<style scoped>
.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.skill-category {
  text-align: center;
}

.category-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.skill-category h3 {
  font-size: 1.5rem;
  margin-bottom: 1.5rem;
  color: var(--text-primary);
}

.skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  justify-content: center;
}

.tag {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.2), rgba(6, 182, 212, 0.2));
  color: var(--accent-cyan);
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-size: 0.9rem;
  font-weight: 500;
  border: 1px solid rgba(6, 182, 212, 0.3);
  transition: all 0.3s ease;
}

.tag:hover {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.3), rgba(6, 182, 212, 0.3));
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(6, 182, 212, 0.2);
}

@media (max-width: 768px) {
  .skills-grid {
    grid-template-columns: 1fr;
  }
}
</style>
