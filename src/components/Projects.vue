<template>
  <section id="projects" class="projects">
    <h2>Featured Projects</h2>
    <div class="projects-container">
      
      <!-- Bliklan Project -->
      <div class="project-card card">
        <div class="project-header">
          <div class="title-row">
            <h3>Bliklan – Blibli Ads System</h3>
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
            <h4>🎯 Problem</h4>
            <p>Legacy budget-constrained ad campaign models (daily/total limits) restricted merchant flexibility and limited platform revenue potential. Additionally, shared Apache Solr infrastructure created dependencies and scalability bottlenecks.</p>
          </div>
          <div class="project-section">
            <h4>💡 Solution</h4>
            <p>Designed and implemented UNLIMITED ad campaigns with credit-threshold-based delivery, replacing budget constraints. Optimized Apache Solr queries, eliminated redundant caches, and contributed to architecture redesign to decouple Solr from central Search team, enabling independent infrastructure management.</p>
          </div>
          <div class="project-section">
            <h4>📈 Impact</h4>
            <ul>
              <li>Reduced API response time from <strong>700ms to 550ms</strong> (21% improvement)</li>
              <li>Improved <strong>merchant flexibility</strong> with unlimited campaign support</li>
              <li>Enhanced <strong>campaign continuity</strong> and platform revenue potential</li>
              <li>Achieved <strong>service isolation and deployment autonomy</strong> through Solr decoupling</li>
            </ul>
          </div>
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

      <!-- Apple Reseller Project -->
      <div class="project-card card">
        <div class="project-header">
          <div class="title-row">
            <h3>Apple Reseller - Loyalty & Rewards System</h3>
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
            <h4>🎯 Problem</h4>
            <p>Merchants needed a streamlined way to process Apple product loyalty claims and cashback requests. Manual IMEI validation was prone to errors and fraud, while reward calculations were time-consuming.</p>
          </div>
          <div class="project-section">
            <h4>💡 Solution</h4>
            <p>Built a Vue.js frontend with barcode scanning feature for merchants to scan Apple product IMEIs. Integrated real-time validation to ensure accuracy and prevent fraudulent claims. Automated reward distribution logic with intelligent point calculations.</p>
          </div>
          <div class="project-section">
            <h4>📈 Impact</h4>
            <ul>
              <li>Enabled <strong>seamless loyalty point claims</strong> and cashback requests</li>
              <li>Implemented <strong>real-time IMEI validation</strong> preventing fraud</li>
              <li>Automated reward calculations improving <strong>dealer retention</strong></li>
              <li>Enhanced merchant experience with intuitive barcode scanning</li>
            </ul>
          </div>
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

      <!-- Assortment and Price Benchmarking Project -->
      <div class="project-card card">
        <div class="project-header">
          <div class="title-row">
            <h3>Assortment & Price Benchmarking Automation</h3>
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
            <h4>🎯 Problem</h4>
            <p>Manual competitor price benchmarking and product mapping across multiple categories was time-consuming, error-prone, and prevented data-driven pricing strategies. Market intelligence gathering required significant human effort.</p>
          </div>
          <div class="project-section">
            <h4>💡 Solution</h4>
            <p>Automated competitor web crawling and product data extraction using Apache JMeter with rotating proxy IPs. Implemented Apache Solr-based product mapping to align competitor products with internal catalogs. Built cron-based scheduling for continuous market intelligence.</p>
          </div>
          <div class="project-section">
            <h4>📈 Impact</h4>
            <ul>
              <li>Eliminated <strong>100% manual effort</strong> in grocery product mapping</li>
              <li>Enabled <strong>scalable and accurate market intelligence</strong> gathering</li>
              <li>Supported <strong>dynamic pricing strategies</strong> and revenue-driven decisions</li>
              <li>Automated batch processing with cron-based scheduling</li>
            </ul>
          </div>
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
  </section>
</template>

<script>
export default {
  name: 'Projects'
}
</script>

<style scoped>
.projects-container {
  display: flex;
  flex-direction: column;
  gap: 2.5rem;
}

.project-card {
  border-left: 4px solid var(--accent-blue);
}

.project-header {
  margin-bottom: 1.5rem;
}

.title-row {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-bottom: 1rem;
  flex-wrap: wrap;
}

.project-header h3 {
  font-size: 1.8rem;
  color: var(--text-primary);
  margin: 0;
}

.role-badge {
  font-size: 0.75rem;
  padding: 0.4rem 0.9rem;
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
  padding: 0.4rem 0.8rem;
  border-radius: 6px;
  font-size: 0.85rem;
  font-weight: 500;
  border: 1px solid rgba(139, 92, 246, 0.3);
}

.project-content {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  margin-bottom: 2rem;
}

.project-section h4 {
  font-size: 1.1rem;
  color: var(--accent-cyan);
  margin-bottom: 0.5rem;
}

.project-section p {
  color: var(--text-secondary);
  line-height: 1.6;
}

.project-section ul {
  list-style: none;
  padding-left: 0;
}

.project-section li {
  color: var(--text-secondary);
  padding: 0.5rem 0;
  padding-left: 1.5rem;
  position: relative;
}

.project-section li::before {
  content: '✓';
  position: absolute;
  left: 0;
  color: var(--accent-cyan);
  font-weight: bold;
}

.project-section strong {
  color: var(--accent-cyan);
  font-weight: 600;
}

.project-metrics {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1.5rem;
  padding-top: 1.5rem;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
}

.metric {
  text-align: center;
}

.metric-value {
  display: block;
  font-size: 2rem;
  font-weight: 700;
  background: linear-gradient(135deg, var(--accent-blue), var(--accent-cyan));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 0.5rem;
}

.metric-label {
  display: block;
  font-size: 0.9rem;
  color: var(--text-secondary);
}

@media (max-width: 768px) {
  .project-header h3 {
    font-size: 1.5rem;
  }

  .title-row {
    flex-direction: column;
    align-items: flex-start;
  }

  .project-metrics {
    grid-template-columns: 1fr 1fr;
  }
}
</style>
