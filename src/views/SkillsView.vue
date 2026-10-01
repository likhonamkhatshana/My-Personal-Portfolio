<script setup>
import { skills } from '../data/portfolio.js'
</script>

<template>
  <section class="page-hero">
    <div class="container narrow">
      <p class="eyebrow">SKILLS</p>
      <h1>What I'm learning.</h1>
      <p>A snapshot of the technical and professional skills I am developing.</p>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <div class="section-heading">
        <p class="eyebrow">TECHNICAL SKILLS</p>
        <h2>My current toolkit.</h2>
      </div>

      <div class="skills-panel glass-card">
        <div v-for="skill in skills" :key="skill.name" class="skill-row">
          <div class="skill-label">
            <strong>{{ skill.name }}</strong>
            <span>{{ skill.status }}</span>
          </div>
          <div class="progress-track" :aria-label="`${skill.name} ${skill.level}%`">
            <span :style="{ width: `${skill.level}%` }"></span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="section section-muted">
    <div class="container">
      <div class="section-heading">
        <p class="eyebrow">TECHNOLOGIES</p>
        <h2>What I use to build.</h2>
      </div>

      <div class="card-grid four">
        <article class="glass-card"><span class="card-number">01</span><h3>HTML5</h3><p>Creating semantic and structured web pages.</p></article>
        <article class="glass-card"><span class="card-number">02</span><h3>CSS3</h3><p>Building layouts, responsive designs and visual systems.</p></article>
        <article class="glass-card"><span class="card-number">03</span><h3>JavaScript</h3><p>Adding interactivity, logic and API communication.</p></article>
        <article class="glass-card"><span class="card-number">04</span><h3>GitHub</h3><p>Managing projects and practicing version control.</p></article>
        <article class="glass-card"><span class="card-number">05</span><h3>Vue.js</h3><p>Learning component-based frontend development.</p></article>
        <article class="glass-card"><span class="card-number">06</span><h3>MySQL</h3><p>Learning how applications store and retrieve data.</p></article>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <div class="section-heading">
        <p class="eyebrow">PROFESSIONAL SKILLS</p>
        <h2>How I work.</h2>
      </div>

      <div class="card-grid four">
        <article class="glass-card"><h3>Teamwork</h3><p>Collaborating effectively with others.</p></article>
        <article class="glass-card"><h3>Communication</h3><p>Sharing ideas clearly and confidently.</p></article>
        <article class="glass-card"><h3>Problem Solving</h3><p>Breaking problems down into practical steps.</p></article>
        <article class="glass-card"><h3>Adaptability</h3><p>Learning and adjusting to new challenges.</p></article>
      </div>
    </div>
  </section>
</template>
