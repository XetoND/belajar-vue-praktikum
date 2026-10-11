<template>
  <div class="home-page">
    <section class="hero-section">
      <div class="hero-content">
        <h1 class="hero-title">
          Connect, Discover, and<br />
          Experience
        </h1>
        <p class="hero-subtitle">
          A community event platform designed to bring ideas together.<br />
          Discover hundreds of events near you.
        </p>
        <div class="hero-action">
          <router-link to="/browse/events" class="btn-primary">Discover Events</router-link>
        </div>
      </div>
    </section>

    <section class="features-section">
      <div class="features-header">
        <h2>Why Choose Gatherly?</h2>
        <p>Everything you need to host or attend unforgettable events.</p>
      </div>

      <div class="features-grid">
        <div class="feature-card">
          <div class="feature-icon">🔍</div>
          <h3>Discover Easily</h3>
          <p>Find events tailored to your interests using our smart category and location filters.</p>
        </div>

        <div class="feature-card">
          <div class="feature-icon">🎟️</div>
          <h3>Seamless Ticketing</h3>
          <p>Register with one click and get your digital QR ticket instantly on your device.</p>
        </div>

        <div class="feature-card">
          <div class="feature-icon">📊</div>
          <h3>Host Like a Pro</h3>
          <p>Manage attendees, track revenue, and scan QR codes with our comprehensive dashboard.</p>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.hero-section {
  /* The Fold & Centered Hero Card */
  min-height: 70vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 5rem 2rem;
  background: #fdfdfd;
  border-radius: 24px;
  border: 1px solid #f0f0f0;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.02);
}

.hero-content {
  max-width: 800px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.hero-title {
  font-size: 3.8rem;
  font-weight: 800;
  line-height: 1.2;
  color: #1c1948;
  margin-bottom: 1.5rem;
  letter-spacing: -0.02em;
}

.hero-subtitle {
  font-size: 1.15rem;
  color: #666;
  line-height: 1.7;
  margin-bottom: 2.5rem;
  max-width: 600px;
}

.hero-action {
  display: flex;
  justify-content: center;
}

.btn-primary {
  display: inline-block;
  padding: 0.9rem 2.4rem;
  font-size: 1.05rem;
  border-radius: 12px;
  font-weight: 600;
  text-decoration: none;
  background: #6644ff;
  color: white;
  box-shadow: 0 6px 20px rgba(102, 68, 255, 0.35);
  transition: all 0.3s ease;
}
.btn-primary:hover {
  background: #5533ee;
  transform: translateY(-2px);
  box-shadow: 0 8px 25px rgba(102, 68, 255, 0.45);
}

.features-grid {
  /* Grid System layout for feature cards */
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: var(--space-8);
}

.home-page {
  display: flex;
  flex-direction: column;
  gap: 4rem;
  animation: fadeIn 0.5s ease;
}

.btn-secondary {
  background: white;
  color: #1c1948;
  border: 1px solid #e0e0e0;
}
.btn-secondary:hover {
  border-color: #6644ff;
  color: #6644ff;
  transform: translateY(-2px);
}

.features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.feature-card {
  background: white;
  padding: 2.5rem;
  border-radius: 16px;
  border: 1px solid #f0f0f0;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.02);
  transition: all 0.3s ease;
  text-align: center;
}
.feature-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.05);
  border-color: #e0e0e0;
}

.feature-icon {
  font-size: 2.5rem;
  margin-bottom: 1.5rem;
}

.feature-card h3 {
  color: #1c1948;
  margin-bottom: 1rem;
  font-size: 1.3rem;
}

.feature-card p {
  color: #666;
  line-height: 1.6;
}

.sitemap-visual {
  padding: 3rem;
  background: #fafafa;
  border-radius: 16px;
  border: 1px solid #f0f0f0;
}
.sitemap-visual h2 {
  color: #1c1948;
  margin-bottom: 0.5rem;
}
.sitemap-desc {
  color: #666;
  margin-bottom: 2.5rem;
}

.tree,
.tree ul {
  list-style: none;
  padding-left: 20px;
}
.tree li {
  margin: 12px 0;
  position: relative;
}
.tree li::before {
  content: '';
  position: absolute;
  top: -12px;
  left: -15px;
  border-left: 1px solid #ddd;
  border-bottom: 1px solid #ddd;
  width: 10px;
  height: 30px;
}
.tree a {
  text-decoration: none;
  color: #444;
  font-weight: 500;
  padding: 8px 16px;
  border-radius: 8px;
  display: inline-block;
  transition: all 0.2s;
  background: white;
  border: 1px solid #eee;
}
.tree a:hover {
  border-color: #ccc;
  color: #1c1948;
}
.tree .router-link-exact-active {
  background: #6644ff;
  color: white;
  border-color: #6644ff;
}

@media (max-width: 768px) {
  .hero-title {
    font-size: 2.5rem;
  }
  .hero-actions {
    flex-direction: column;
    width: 100%;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>