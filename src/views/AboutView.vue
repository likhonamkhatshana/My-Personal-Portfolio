<script setup>
import { interests } from '../data/portfolio.js'
</script>

<template>
  <section class="page-hero">
    <div class="container narrow">
      <p class="eyebrow">ABOUT ME</p>
      <h1>Who I am & where I'm going.</h1>
      <p>
        Get to know who I am, what inspires me, and where I am heading in my
        technology journey.
      </p>
    </div>
  </section>

  <section class="section">
    <div class="container two-column">
      <article class="glass-card">
        <p class="card-kicker">WHO AM I?</p>
        <h2>An aspiring developer with a curious mind.</h2>
        <p>
          My name is Likona Mkhatshana and I am an aspiring software developer
          with a growing passion for technology, problem solving and web
          development.
        </p>
        <p>
          I enjoy learning new concepts, building projects and challenging
          myself to improve. Through practice and persistence, I am developing
          the skills needed to grow in the ICT industry.
        </p>
      </article>

      <article class="quote-card">
        <span>“</span>
        <p>
          Every project teaches me something new and brings me one step closer
          to becoming a professional developer.
        </p>
      </article>
    </div>
  </section>

  <section class="section section-muted">
    <div class="container">
      <div class="section-heading">
        <p class="eyebrow">WHAT INTERESTS ME</p>
        <h2>Things I enjoy exploring.</h2>
      </div>

      <div class="card-grid four">
        <article v-for="interest in interests" :key="interest.title" class="glass-card">
          <span class="card-number">0{{ interests.indexOf(interest) + 1 }}</span>
          <h3>{{ interest.title }}</h3>
          <p>{{ interest.text }}</p>
        </article>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <div class="section-heading">
        <p class="eyebrow">LEARNING JOURNEY</p>
        <h2>From first concepts to real projects.</h2>
      </div>

      <div class="timeline">
        <article class="timeline-item">
          <span>2026</span>
          <div>
            <h3>ICT Training</h3>
            <p>Started my formal ICT training journey and began exploring the world of technology.</p>
          </div>
        </article>
        <article class="timeline-item">
          <span>01</span>
          <div>
            <h3>HTML & CSS</h3>
            <p>Learned how to structure webpages and create responsive layouts.</p>
          </div>
        </article>
        <article class="timeline-item">
          <span>02</span>
          <div>
            <h3>JavaScript</h3>
            <p>Started learning programming concepts, functions, arrays and problem solving.</p>
          </div>
        </article>
        <article class="timeline-item">
          <span>03</span>
          <div>
            <h3>APIs & Backend</h3>
            <p>Started connecting applications to APIs, databases and server-side code.</p>
          </div>
        </article>
        <article class="timeline-item">
          <span>04</span>
          <div>
            <h3>Vue.js</h3>
            <p>Moved my portfolio into Vue to learn components, routing and reusable UI.</p>
          </div>
        </article>
      </div>
    </div>
  </section>

  <section class="section section-muted">
    <div class="container">
      <div class="section-heading">
        <p class="eyebrow">EDUCATION & LEARNING</p>
        <h2>What I'm working through.</h2>
      </div>

      <div class="table-wrap">
        <table>
          <thead>
            <tr><th>Course</th><th>Status</th></tr>
          </thead>
          <tbody>
            <tr><td>HTML & CSS</td><td>Completed</td></tr>
            <tr><td>JavaScript Fundamentals</td><td>In progress</td></tr>
            <tr><td>Vue.js</td><td>In progress</td></tr>
            <tr><td>MySQL</td><td>In progress</td></tr>
            <tr><td>ICT Training</td><td>In progress</td></tr>
          </tbody>
        </table>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container glass-card reflection">
      <p class="card-kicker">REFLECTION</p>
      <h2>Still learning. Still building.</h2>
      <p>
        When I first started learning web development, many concepts seemed
        difficult and unfamiliar. Through practice, teamwork, persistence and
        problem-solving, I have become more confident in my abilities.
      </p>
      <p>
        This portfolio is not only a collection of work but also a
        representation of my growth, determination and commitment to continuous
        learning.
      </p>
    </div>
  </section>
</template>
