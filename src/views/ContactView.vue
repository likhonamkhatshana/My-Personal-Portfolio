<script setup>
import SocialLinks from '../components/SocialLinks.vue'
</script>

<template>
  <section class="page-hero">
    <div class="container narrow">
      <p class="eyebrow">CONTACT</p>
      <h1>Let's talk.</h1>
      <p>
        Feel free to contact me for collaboration, networking or opportunities.
      </p>
    </div>
  </section>

  <section class="section">
    <div class="container contact-grid">
      <div>
        <p class="eyebrow">GET IN TOUCH</p>
        <h2>Have an idea, opportunity or question?</h2>
        <p class="section-text">
          Send me a message through the form. The form is handled by Formspree,
          so you do not need a custom backend just to receive portfolio
          enquiries.
        </p>

        <SocialLinks />
      </div>

      <form
        class="contact-form glass-card"
        action="https://formspree.io/f/moevbogq"
        method="POST"
      >
        <input type="hidden" name="_subject" value="New portfolio enquiry" />

        <label for="name">Name</label>
        <input
          id="name"
          name="name"
          type="text"
          autocomplete="name"
          placeholder="Your name"
          required
        />

        <label for="email">Email</label>
        <input
          id="email"
          name="email"
          type="email"
          autocomplete="email"
          placeholder="you@example.com"
          required
        />

        <label for="message">Message</label>
        <textarea
          id="message"
          name="message"
          rows="7"
          placeholder="Tell me a little about what you would like to discuss..."
          required
        ></textarea>

        <button class="button button-primary" type="submit">
          Send message ↗
        </button>

      </form>
    </div>
  </section>
</template>
