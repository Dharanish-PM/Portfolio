<template>
  <section 
    id="education" 
    class="education"
    v-motion
    :initial="{ opacity: 0, y: 50 }"
    :visible="{ opacity: 1, y: 0, transition: { duration: 600, ease: 'easeOut' } }"
  >
    <h2>Education</h2>
    <div class="education-grid">
      <div class="education-card card">
        <div class="education-icon">🎓</div>
        <div class="education-content">
          <h3>MSc in Cloud Computing</h3>
          <h4>National College of Ireland</h4>
          <p class="duration">Currently Pursuing (Expected Jan 2027)</p>
          <p class="visa-status">📍 Based in Ireland | Stamp 2 Visa with Part-time Work Eligibility</p>
          <p class="description">
            Advanced studies in cloud architecture, distributed systems, containerization, 
            and modern DevOps practices. Focus on AWS, Azure, Kubernetes, and cloud-native application development.
          </p>
          <div class="highlights">
            <span class="highlight">☁️ Cloud Architecture</span>
            <span class="highlight">🐳 Kubernetes</span>
            <span class="highlight">🔧 DevOps</span>
            <span class="highlight">📊 Distributed Systems</span>
          </div>
        </div>
      </div>

      <div class="education-card card">
        <div class="education-icon">🎓</div>
        <div class="education-content">
          <h3>B.E. Computer Science and Engineering</h3>
          <h4>University Name</h4>
          <p class="duration">Graduated: 2021</p>
          <p class="cgpa">CGPA: <strong>8.90 / 10.0</strong></p>
          <p class="description">
            Strong foundation in computer science fundamentals including data structures, 
            algorithms, database systems, software engineering, and web technologies.
          </p>
          <div class="highlights">
            <span class="highlight">💻 Software Engineering</span>
            <span class="highlight">🗄️ Database Systems</span>
            <span class="highlight">🔍 Algorithms</span>
            <span class="highlight">🌐 Web Technologies</span>
          </div>
        </div>
      </div>
    </div>

    <div class="learning-section">
      <h3>Currently Learning</h3>
      <div class="learning-items">
        <div class="learning-item">
          <span class="learning-icon">☁️</span>
          <div>
            <h4>Advanced Cloud Computing</h4>
            <p>Deep diving into cloud-native architectures and serverless computing</p>
          </div>
        </div>
        <div class="learning-item">
          <span class="learning-icon">🚢</span>
          <div>
            <h4>Kubernetes & Container Orchestration</h4>
            <p>Mastering container orchestration and microservices deployment</p>
          </div>
        </div>
        <div class="learning-item">
          <span class="learning-icon">🔐</span>
          <div>
            <h4>Cloud Security & Best Practices</h4>
            <p>Implementing secure, scalable cloud infrastructure</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Education'
}
</script>

<style scoped>
.education-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
  gap: 2rem;
  margin-bottom: 4rem;
}

.education-card {
  display: flex;
  gap: 1.5rem;
}

.education-icon {
  font-size: 3rem;
  flex-shrink: 0;
}

.education-content h3 {
  font-size: 1.5rem;
  color: var(--text-primary);
  margin-bottom: 0.5rem;
}

.education-content h4 {
  font-size: 1.1rem;
  color: var(--accent-cyan);
  font-weight: 500;
  margin-bottom: 0.5rem;
}

.duration {
  color: var(--text-secondary);
  font-size: 0.95rem;
  margin-bottom: 0.5rem;
}

.visa-status {
  color: var(--accent-cyan);
  font-size: 0.95rem;
  font-weight: 600;
  margin-bottom: 1rem;
  padding: 0.5rem 0.75rem;
  background: rgba(6, 182, 212, 0.1);
  border-left: 3px solid var(--accent-cyan);
  border-radius: 4px;
  display: inline-block;
}

.cgpa {
  color: var(--text-secondary);
  font-size: 1rem;
  margin-bottom: 1rem;
}

.cgpa strong {
  color: var(--accent-cyan);
  font-size: 1.2rem;
}

.description {
  color: var(--text-secondary);
  line-height: 1.6;
  margin-bottom: 1rem;
}

.highlights {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.highlight {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.2), rgba(6, 182, 212, 0.2));
  color: var(--accent-cyan);
  padding: 0.4rem 0.8rem;
  border-radius: 6px;
  font-size: 0.85rem;
  font-weight: 500;
  border: 1px solid rgba(6, 182, 212, 0.3);
}

.learning-section {
  background: var(--bg-card);
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 6px var(--shadow);
}

.learning-section h3 {
  font-size: 1.8rem;
  color: var(--text-primary);
  margin-bottom: 2rem;
  text-align: center;
}

.learning-items {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
}

.learning-item {
  display: flex;
  gap: 1rem;
  align-items: start;
  padding: 1.5rem;
  background: rgba(59, 130, 246, 0.1);
  border-radius: 8px;
  border-left: 3px solid var(--accent-blue);
  transition: transform 0.3s ease;
}

.learning-item:hover {
  transform: translateX(5px);
}

.learning-icon {
  font-size: 2rem;
  flex-shrink: 0;
}

.learning-item h4 {
  font-size: 1.1rem;
  color: var(--text-primary);
  margin-bottom: 0.5rem;
}

.learning-item p {
  color: var(--text-secondary);
  font-size: 0.95rem;
  line-height: 1.5;
}

@media (max-width: 768px) {
  .education-grid {
    grid-template-columns: 1fr;
  }

  .learning-items {
    grid-template-columns: 1fr;
  }
}
</style>
