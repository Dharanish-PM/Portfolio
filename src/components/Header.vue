<template>
  <header :class="{ scrolled: isScrolled }">
    <div class="container">
      <div class="logo">
        <span class="logo-text">&lt;Dev/&gt;</span>
      </div>
      <nav :class="{ active: menuOpen }">
        <a href="#hero" @click="closeMenu">Home</a>
        <a href="#about" @click="closeMenu">About</a>
        <a href="#skills" @click="closeMenu">Skills</a>
        <a href="#experience" @click="closeMenu">Experience</a>
        <a href="#education" @click="closeMenu">Education</a>
        <a href="#contact" @click="closeMenu">Contact</a>
      </nav>
      <button class="menu-toggle" @click="toggleMenu">
        <span></span>
        <span></span>
        <span></span>
      </button>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      isScrolled: false,
      menuOpen: false
    }
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll)
  },
  beforeUnmount() {
    window.removeEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      this.isScrolled = window.scrollY > 50
    },
    toggleMenu() {
      this.menuOpen = !this.menuOpen
    },
    closeMenu() {
      this.menuOpen = false
    }
  }
}
</script>

<style scoped>
header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
  padding: 1.5rem 0;
  transition: all 0.3s ease;
  background: rgba(15, 23, 42, 0.8);
  backdrop-filter: blur(10px);
}

header.scrolled {
  padding: 1rem 0;
  background: rgba(15, 23, 42, 0.95);
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo-text {
  font-size: 1.5rem;
  font-weight: 700;
  background: linear-gradient(135deg, var(--accent-blue), var(--accent-cyan));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

nav {
  display: flex;
  gap: 2rem;
}

nav a {
  color: var(--text-secondary);
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
  position: relative;
}

nav a::after {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--accent-blue);
  transition: width 0.3s ease;
}

nav a:hover {
  color: var(--text-primary);
}

nav a:hover::after {
  width: 100%;
}

.menu-toggle {
  display: none;
  flex-direction: column;
  gap: 5px;
  background: none;
  border: none;
  cursor: pointer;
}

.menu-toggle span {
  width: 25px;
  height: 3px;
  background: var(--text-primary);
  transition: all 0.3s ease;
}

@media (max-width: 768px) {
  .menu-toggle {
    display: flex;
  }

  nav {
    position: fixed;
    top: 70px;
    right: -100%;
    flex-direction: column;
    background: var(--bg-secondary);
    padding: 2rem;
    border-radius: 12px;
    box-shadow: 0 4px 6px var(--shadow);
    transition: right 0.3s ease;
  }

  nav.active {
    right: 20px;
  }
}
</style>
