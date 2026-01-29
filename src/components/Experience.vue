<template>
  <section 
    id="experience" 
    class="experience"
    v-motion
    :initial="{ opacity: 0, y: 50 }"
    :visible="{ opacity: 1, y: 0, transition: { duration: 600, ease: 'easeOut' } }"
  >
    <h2>Experience & Projects</h2>
    <div class="timeline">
      <div class="timeline-item">
        <div class="timeline-marker"></div>
        <div class="timeline-content card">
          <div class="timeline-header">
            <div>
              <h3>Software Engineer</h3>
              <h4>Quinbay Technologies (Blibli.com)</h4>
              <p class="location">Indonesian-based E-commerce Company</p>
            </div>
            <span class="timeline-date">Aug 2024 - Nov 2025</span>
          </div>
          <p class="company-description">
            Quinbay Technologies is a prominent Indonesian e-commerce firm with a wide product portfolio and an extensive nationwide distribution network, recognized as one of Indonesia's largest e-commerce platforms.
          </p>

          <!-- Bliklan Project -->
          <div class="project-card">
            <div class="project-header">
              <div class="title-row">
                <h4 class="project-title">🔹 Bliklan – Blibli Ads System</h4>
                <span class="role-badge">Backend</span>
              </div>
              <div class="project-tags">
                <span class="tech-tag">Java</span>
                <span class="tech-tag">Spring Boot</span>
                <span class="tech-tag">Apache Solr</span>
                <span class="tech-tag">Microservices</span>
                <span class="tech-tag">Redis</span>
              </div>
            </div>
            <div class="project-content">
              <div class="project-section">
                <h5>🎯 Problem</h5>
                <p>Legacy budget-constrained ad campaign models (daily/total limits) restricted merchant flexibility and limited platform revenue potential. Additionally, shared Apache Solr infrastructure created dependencies and scalability bottlenecks.</p>
              </div>
              <div class="project-section">
                <h5>💡 Solution</h5>
                <ul class="responsibilities">
                  <li>Designed and implemented support for <strong>UNLIMITED ad campaigns</strong>, enabling continuous ad delivery until a configurable credit threshold is reached. Replaced legacy budget-constrained models, improving merchant flexibility, campaign continuity, and platform revenue potential</li>
                  <li>Optimized Apache Solr queries and eliminated redundant caches, reduced average response time from <strong>700ms to 550ms</strong> and significantly improving system performance and user experience</li>
                  <li>Contributed to architecture redesign to decouple Apache Solr from the central Search team, enabling Bliklan to own and manage its independent search infrastructure. Worked on migrating from a shared Solr dependency to a dedicated Solr setup, improving service isolation, scalability, and deployment autonomy</li>
                </ul>
              </div>
              <div class="project-metrics">
                <div class="metric">
                  <span class="metric-value">21%</span>
                  <span class="metric-label">Faster Response</span>
                </div>
                <div class="metric">
                  <span class="metric-value">550ms</span>
                  <span class="metric-label">API Response Time</span>
                </div>
                <div class="metric">
                  <span class="metric-value">∞</span>
                  <span class="metric-label">Campaigns</span>
                </div>
              </div>
            </div>
          </div>

          <!-- Apple Reseller Project -->
          <div class="project-card">
            <div class="project-header">
              <div class="title-row">
                <h4 class="project-title">🔹 Apple Reseller - Loyalty & Rewards</h4>
                <span class="role-badge frontend">Frontend - Vue.js</span>
              </div>
              <div class="project-tags">
                <span class="tech-tag">Vue.js</span>
                <span class="tech-tag">JavaScript</span>
                <span class="tech-tag">REST APIs</span>
                <span class="tech-tag">Real-time Validation</span>
              </div>
            </div>
            <div class="project-content">
              <div class="project-section">
                <h5>🎯 Problem</h5>
                <p>Merchants needed a streamlined way to process Apple product loyalty claims and cashback requests. Manual IMEI validation was prone to errors and fraud, while reward calculations were time-consuming.</p>
              </div>
              <div class="project-section">
                <h5>💡 Solution</h5>
                <ul class="responsibilities">
                  <li>Implemented a <strong>barcode scanning feature</strong> for merchants to scan Apple product IMEIs, enabling seamless loyalty point claims and cashback requests</li>
                  <li>Integrated <strong>real-time validation</strong> of scanned IMEIs, ensuring accuracy and preventing fraudulent claims</li>
                  <li>Optimized reward distribution logic, automating point calculations and improving dealer retention</li>
                </ul>
              </div>
              <div class="project-metrics">
                <div class="metric">
                  <span class="metric-value">100%</span>
                  <span class="metric-label">Real-time Validation</span>
                </div>
                <div class="metric">
                  <span class="metric-value">↑</span>
                  <span class="metric-label">Dealer Retention</span>
                </div>
                <div class="metric">
                  <span class="metric-value">0</span>
                  <span class="metric-label">Fraud Claims</span>
                </div>
              </div>
            </div>
          </div>

          <div class="tech-stack-summary">
            <h5>Technologies Used</h5>
            <div class="tech-stack">
              <span class="tech">Java</span>
              <span class="tech">Spring Boot</span>
              <span class="tech">Vue.js</span>
              <span class="tech">Apache Solr</span>
              <span class="tech">Microservices</span>
              <span class="tech">RESTful APIs</span>
              <span class="tech">Apache Kafka</span>
              <span class="tech">Redis</span>
              <span class="tech">MySQL</span>
              <span class="tech">MongoDB</span>
              <span class="tech">AWS</span>
              <span class="tech">Docker</span>
              <span class="tech">Jenkins</span>
              <span class="tech">CI/CD</span>
              <span class="tech">Git</span>
            </div>
          </div>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-marker"></div>
        <div class="timeline-content card">
          <div class="timeline-header">
            <div>
              <h3>Software Engineer Intern</h3>
              <h4>Quinbay Technologies (Blibli.com)</h4>
              <p class="location">Coimbatore, India</p>
            </div>
            <span class="timeline-date">Dec 2023 - Jul 2024</span>
          </div>

          <!-- Assortment and Price Benchmarking Project -->
          <div class="project-card">
            <div class="project-header">
              <div class="title-row">
                <h4 class="project-title">🔹 Assortment & Price Benchmarking</h4>
                <span class="role-badge">Backend</span>
              </div>
              <div class="project-tags">
                <span class="tech-tag">Java</span>
                <span class="tech-tag">Apache JMeter</span>
                <span class="tech-tag">Apache Solr</span>
                <span class="tech-tag">Web Crawling</span>
                <span class="tech-tag">Cron Jobs</span>
              </div>
            </div>
            <div class="project-content">
              <div class="project-section">
                <h5>🎯 Problem</h5>
                <p>Manual competitor price benchmarking and product mapping across multiple categories was time-consuming, error-prone, and prevented data-driven pricing strategies. Market intelligence gathering required significant human effort.</p>
              </div>
              <div class="project-section">
                <h5>💡 Solution</h5>
                <ul class="responsibilities">
                  <li>Automated competitor web crawling and product data extraction across multiple categories using <strong>Apache JMeter</strong> and rotating proxy IPs, enabling scalable and accurate market intelligence</li>
                  <li>Implemented <strong>Apache Solr-based product mapping</strong> to align competitor products with internal catalogs, supporting price benchmarking, dynamic pricing strategies, and revenue-driven decision making</li>
                  <li>Fully automated grocery product mapping workflows, eliminating <strong>100% manual effort</strong> through cron-based scheduling and batch processing</li>
                </ul>
              </div>
              <div class="project-metrics">
                <div class="metric">
                  <span class="metric-value">100%</span>
                  <span class="metric-label">Automation</span>
                </div>
                <div class="metric">
                  <span class="metric-value">0</span>
                  <span class="metric-label">Manual Effort</span>
                </div>
                <div class="metric">
                  <span class="metric-value">24/7</span>
                  <span class="metric-label">Market Intelligence</span>
                </div>
              </div>
            </div>
          </div>

          <div class="tech-stack-summary">
            <h5>Technologies Used</h5>
            <div class="tech-stack">
              <span class="tech">Java</span>
              <span class="tech">Spring Boot</span>
              <span class="tech">Apache JMeter</span>
              <span class="tech">Apache Solr</span>
              <span class="tech">REST APIs</span>
              <span class="tech">MySQL</span>
              <span class="tech">Cron Jobs</span>
              <span class="tech">Git</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Experience'
}
</script>

<style scoped>
.experience {
  background: rgba(30, 41, 59, 0.3);
  border-radius: 20px;
  margin: 2rem auto;
}

.timeline {
  position: relative;
  padding-left: 2rem;
}

.timeline::before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  width: 2px;
  background: linear-gradient(180deg, var(--accent-blue), var(--accent-cyan));
}

.timeline-item {
  position: relative;
  margin-bottom: 3rem;
}

.timeline-item:last-child {
  margin-bottom: 0;
}

.timeline-marker {
  position: absolute;
  left: -2.5rem;
  top: 0;
  width: 16px;
  height: 16px;
  border-radius: 50%;
  background: var(--accent-cyan);
  border: 3px solid var(--bg-primary);
  box-shadow: 0 0 0 4px rgba(6, 182, 212, 0.2);
}

.timeline-content {
  margin-left: 2rem;
}

.timeline-header {
  display: flex;
  justify-content: space-between;
  align-items: start;
  margin-bottom: 1.5rem;
  flex-wrap: wrap;
  gap: 1rem;
}

.timeline-header h3 {
  font-size: 1.5rem;
  color: var(--text-primary);
  margin-bottom: 0.5rem;
}

.timeline-header h4 {
  font-size: 1.1rem;
  color: var(--accent-cyan);
  font-weight: 500;
}

.location {
  font-size: 0.95rem;
  color: var(--text-secondary);
  font-style: italic;
  margin-top: 0.25rem;
}

.company-description {
  color: var(--text-secondary);
  line-height: 1.6;
  margin-bottom: 2rem;
  font-style: italic;
  padding: 1rem;
  background: rgba(59, 130, 246, 0.05);
  border-left: 3px solid var(--accent-blue);
  border-radius: 4px;
}

.timeline-date {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.2), rgba(6, 182, 212, 0.2));
  color: var(--accent-cyan);
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-size: 0.9rem;
  font-weight: 600;
  border: 1px solid rgba(6, 182, 212, 0.3);
  white-space: nowrap;
}

/* Project Cards */
.project-card {
  margin-bottom: 2rem;
  padding: 2rem;
  background: rgba(15, 23, 42, 0.5);
  border-radius: 12px;
  border-left: 4px solid var(--accent-cyan);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
  transform: translateX(5px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
}

.project-header {
  margin-bottom: 1.5rem;
}

.title-row {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  margin-bottom: 1rem;
  flex-wrap: wrap;
}

.project-title {
  font-size: 1.3rem;
  color: var(--text-primary);
  margin: 0;
  font-weight: 600;
}

.role-badge {
  font-size: 0.7rem;
  padding: 0.35rem 0.8rem;
  border-radius: 12px;
  background: linear-gradient(135deg, var(--accent-blue), var(--accent-cyan));
  color: white;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.5px;
  white-space: nowrap;
}

.role-badge.frontend {
  background: linear-gradient(135deg, var(--accent-purple), #a78bfa);
}

.project-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.tech-tag {
  background: rgba(139, 92, 246, 0.2);
  color: var(--accent-purple);
  padding: 0.35rem 0.7rem;
  border-radius: 6px;
  font-size: 0.8rem;
  font-weight: 500;
  border: 1px solid rgba(139, 92, 246, 0.3);
}

.project-content {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.project-section h5 {
  font-size: 1rem;
  color: var(--accent-cyan);
  margin-bottom: 0.5rem;
  font-weight: 600;
}

.project-section p {
  color: var(--text-secondary);
  line-height: 1.6;
  margin: 0;
}

.responsibilities {
  list-style: none;
  padding-left: 0;
  margin: 0;
}

.responsibilities li {
  color: var(--text-secondary);
  padding: 0.5rem 0;
  padding-left: 1.5rem;
  position: relative;
  line-height: 1.6;
}

.responsibilities li::before {
  content: '▹';
  position: absolute;
  left: 0;
  color: var(--accent-cyan);
  font-weight: bold;
  font-size: 1.2rem;
}

.responsibilities li strong {
  color: var(--text-primary);
  font-weight: 600;
}

.project-metrics {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
  gap: 1rem;
  padding-top: 1.5rem;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
}

.metric {
  text-align: center;
}

.metric-value {
  display: block;
  font-size: 1.8rem;
  font-weight: 700;
  background: linear-gradient(135deg, var(--accent-blue), var(--accent-cyan));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 0.3rem;
}

.metric-label {
  display: block;
  font-size: 0.85rem;
  color: var(--text-secondary);
}

.tech-stack-summary {
  margin-top: 1rem;
  padding-top: 1.5rem;
  border-top: 2px solid rgba(255, 255, 255, 0.1);
}

.tech-stack-summary h5 {
  font-size: 1rem;
  color: var(--text-primary);
  margin-bottom: 1rem;
  font-weight: 600;
}

.tech-stack {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.tech {
  background: rgba(139, 92, 246, 0.2);
  color: var(--accent-purple);
  padding: 0.4rem 0.8rem;
  border-radius: 6px;
  font-size: 0.85rem;
  font-weight: 500;
  border: 1px solid rgba(139, 92, 246, 0.3);
}

@media (max-width: 768px) {
  .timeline {
    padding-left: 1.5rem;
  }

  .timeline-content {
    margin-left: 1rem;
  }

  .timeline-marker {
    left: -2.25rem;
  }

  .timeline-header {
    flex-direction: column;
  }

  .timeline-date {
    align-self: flex-start;
  }

  .project-card {
    padding: 1.5rem;
  }

  .project-title {
    font-size: 1.1rem;
  }

  .title-row {
    flex-direction: column;
    align-items: flex-start;
  }

  .project-metrics {
    grid-template-columns: repeat(2, 1fr);
  }
}
</style>
