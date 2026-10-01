<script setup>
import { projects } from '../data/portfolio.js'
import ProjectCard from '../components/ProjectCard.vue'
</script>

<template>
  <section class="page-hero">
    <div class="container narrow">
      <p class="eyebrow">PROJECTS</p>
      <h1>Things I've built.</h1>
      <p>
        A collection of projects that show what I am learning and how my
        skills are developing.
      </p>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <div class="project-grid">
        <ProjectCard
          v-for="project in projects"
          :key="project.title"
          :project="project"
        />
      </div>
    </div>
  </section>

  <section class="section section-muted">
    <div class="container cta-card">
      <p class="eyebrow">NEXT PROJECT</p>
      <h2>Something new is always in progress.</h2>
      <p>
        I am continuing to build, experiment and turn what I learn into
        practical projects.
      </p>
      <RouterLink class="button button-primary" to="/contact">
        Let's connect
      </RouterLink>
    </div>
  </section>
</template>
