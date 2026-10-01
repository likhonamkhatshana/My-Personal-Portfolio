<script setup>
import SocialLinks from '../components/SocialLinks.vue'
</script>

<template>

  <section class="home-hero">

    <div class="container hero-grid">

      <div class="hero-copy">

        <p class="eyebrow">
          ASPIRING SOFTWARE DEVELOPER
        </p>

        <h1>
          Hello, I'm
          <span>Likona.</span>
        </h1>

        <p class="hero-lead">
          I am an ICT learner passionate about web development,
          creativity and problem solving. I am building my skills
          one project at a time.
        </p>


        <div class="hero-actions">

          <RouterLink
            class="button button-primary"
            to="/about"
          >
            More about me
          </RouterLink>


          <RouterLink
            class="button button-outline"
            to="/projects"
          >
            View projects
          </RouterLink>

        </div>


        <SocialLinks compact />

      </div>


      <div class="hero-visual">

        <div class="portrait-frame">

          <img
            src="https://i.ibb.co/HLq77YVS/IMG-20260715-WA0002.jpg"
            alt="Likona Mkhatshana"
          />

        </div>


        <div class="visual-note">

          <span>
            Currently learning
          </span>

          <strong>
            Vue · JavaScript · MySQL
          </strong>

        </div>

      </div>

    </div>

  </section>


  <section class="section section-muted">

    <div class="container intro-grid">

      <div>

        <p class="eyebrow">
          A LITTLE ABOUT ME
        </p>

        <h2>
          Learning with intention.
        </h2>

      </div>


      <p class="section-text">

        My portfolio is a record of where I am now,
        what I have built, and what I am learning next.
        I care about understanding the code behind the
        interface, not just making something that looks good.

      </p>

    </div>

  </section>

</template>