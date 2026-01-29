<template>
  <section 
    id="contact" 
    class="contact"
    v-motion
    :initial="{ opacity: 0, y: 50 }"
    :visible="{ opacity: 1, y: 0, transition: { duration: 600, ease: 'easeOut' } }"
  >
    <h2>Get In Touch</h2>
    <p class="contact-intro">
      I'm currently open to Summer Internship and Software Engineering roles. 
      Let's connect and discuss how I can contribute to your team!
    </p>
    
    <div class="contact-content">
      <div class="contact-info">
        <h3>Contact Information</h3>
        <div class="info-items">
          <a href="mailto:dharanishpm@gmail.com" class="info-item">
            <span class="info-icon">📧</span>
            <div>
              <h4>Email</h4>
              <p>dharanishpm@gmail.com</p>
            </div>
          </a>
          
          <a href="https://github.com/Dharanish-PM" target="_blank" class="info-item">
            <span class="info-icon">💻</span>
            <div>
              <h4>GitHub</h4>
              <p>github.com/Dharanish-PM</p>
            </div>
          </a>
          
          <a href="https://linkedin.com/in/dharanishpm" target="_blank" class="info-item">
            <span class="info-icon">💼</span>
            <div>
              <h4>LinkedIn</h4>
              <p>linkedin.com/in/dharanishpm</p>
            </div>
          </a>
          
          <a href="tel:+353899797636" class="info-item">
            <span class="info-icon">📱</span>
            <div>
              <h4>Phone</h4>
              <p>+353 899797636</p>
            </div>
          </a>
        </div>
      </div>

      <div class="contact-form-container card">
        <h3>Send a Message</h3>
        <form @submit.prevent="handleSubmit" class="contact-form">
          <div class="form-group">
            <label for="name">Name</label>
            <input 
              type="text" 
              id="name" 
              v-model="formData.name" 
              required 
              placeholder="Your Name"
            />
          </div>
          
          <div class="form-group">
            <label for="email">Email</label>
            <input 
              type="email" 
              id="email" 
              v-model="formData.email" 
              required 
              placeholder="your.email@example.com"
            />
          </div>
          
          <div class="form-group">
            <label for="subject">Subject</label>
            <input 
              type="text" 
              id="subject" 
              v-model="formData.subject" 
              required 
              placeholder="What's this about?"
            />
          </div>
          
          <div class="form-group">
            <label for="message">Message</label>
            <textarea 
              id="message" 
              v-model="formData.message" 
              required 
              rows="5"
              placeholder="Your message here..."
            ></textarea>
          </div>

           <p>**Currently under Development**</p>
          <button  type="submit" class="btn btn-primary" disabled="true" >
            {{ isSubmitting ? 'Sending...' : 'Send Message' }}
          </button>
          
          <p v-if="submitMessage" class="submit-message" :class="{ success: submitSuccess }">
            {{ submitMessage }}
          </p>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Contact',
  data() {
    return {
      formData: {
        name: '',
        email: '',
        subject: '',
        message: ''
      },
      isSubmitting: false,
      submitMessage: '',
      submitSuccess: false
    }
  },
  methods: {
    async handleSubmit() {
      // this.isSubmitting = true
      //this.submitMessage = ''
      
      //try {
        // Send to Formspree - Replace with your actual Formspree endpoint
        // Sign up at https://formspree.io and get your form ID
        //const response = await fetch('https://formspree.io/f/YOUR_FORM_ID', {
          //method: 'POST',
          //headers: {
            //'Content-Type': 'application/json'
          //},
          //body: JSON.stringify({
            //name: this.formData.name,
            //email: this.formData.email,
            //subject: this.formData.subject,
            //message: this.formData.message,
            //_replyto: this.formData.email,
            //_to: 'dharanishpriv@gmail.com'
          //})
        //})
        
        //if (response.ok) {
          //this.isSubmitting = false
          //this.submitSuccess = true
          //this.submitMessage = 'Message sent successfully! I\'ll get back to you soon.'
          
          // Reset form
          //this.formData = {
            //name: '',
            //email: '',
            //subject: '',
            //message: ''
          //}
          
          // Clear success message after 5 seconds
          //setTimeout(() => {
            //this.submitMessage = ''
            //this.submitSuccess = false
          //}, 5000)
        //} else {
          //throw new Error('Failed to send message')
        //}
      //} catch (error) {
        //this.isSubmitting = false
        //this.submitSuccess = false
        //this.submitMessage = 'Failed to send message. Please try emailing me directly at dharanishpm@gmail.com'
        
        // Clear error message after 7 seconds
        //setTimeout(() => {
          //this.submitMessage = ''
        //}, 7000)
      //}
    }
  }
}
</script>

<style scoped>
.contact {
  background: rgba(30, 41, 59, 0.3);
  border-radius: 20px;
  margin: 2rem auto;
}

.contact-intro {
  text-align: center;
  font-size: 1.2rem;
  color: var(--text-secondary);
  max-width: 700px;
  margin: 0 auto 3rem;
  line-height: 1.8;
}

.contact-content {
  display: grid;
  grid-template-columns: 1fr 1.5fr;
  gap: 3rem;
  align-items: start;
}

.contact-info h3,
.contact-form-container h3 {
  font-size: 1.5rem;
  color: var(--text-primary);
  margin-bottom: 1.5rem;
}

.info-items {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.info-item {
  display: flex;
  gap: 1rem;
  align-items: start;
  padding: 1.5rem;
  background: var(--bg-card);
  border-radius: 12px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  text-decoration: none;
  color: inherit;
}

.info-item:hover {
  transform: translateX(5px);
  box-shadow: 0 4px 12px var(--shadow);
}

.info-icon {
  font-size: 2rem;
  flex-shrink: 0;
}

.info-item h4 {
  font-size: 1rem;
  color: var(--text-primary);
  margin-bottom: 0.25rem;
}

.info-item p {
  color: var(--accent-cyan);
  font-size: 0.95rem;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.form-group {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.form-group label {
  color: var(--text-primary);
  font-weight: 500;
  font-size: 0.95rem;
}

.form-group input,
.form-group textarea {
  background: rgba(15, 23, 42, 0.5);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 8px;
  padding: 0.75rem 1rem;
  color: var(--text-primary);
  font-family: inherit;
  font-size: 1rem;
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
}

.form-group input:focus,
.form-group textarea:focus {
  outline: none;
  border-color: var(--accent-blue);
  box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.1);
}

.form-group textarea {
  resize: vertical;
  min-height: 120px;
}

.btn[disabled] {
  opacity: 0.6;
  cursor: not-allowed;
}

.submit-message {
  text-align: center;
  padding: 1rem;
  border-radius: 8px;
  background: rgba(239, 68, 68, 0.1);
  color: #ef4444;
  font-weight: 500;
}

.submit-message.success {
  background: rgba(34, 197, 94, 0.1);
  color: #22c55e;
}

@media (max-width: 968px) {
  .contact-content {
    grid-template-columns: 1fr;
  }
}
</style>
