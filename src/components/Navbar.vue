<script setup>
import { ref } from 'vue'

const menuOpen = ref(false)

const closeMenu = () => {
  menuOpen.value = false
}
</script>

<template>

  <header class="site-header">

    <nav class="navbar container">

      <RouterLink
        class="logo"
        to="/"
        @click="closeMenu"
      >
        <span>Likona</span>
        <small>Mkhatshana</small>
      </RouterLink>


      <button
        class="menu-toggle"
        type="button"
        :aria-expanded="menuOpen"
        aria-label="Toggle navigation"
        @click="menuOpen = !menuOpen"
      >

        <span></span>
        <span></span>
        <span></span>

      </button>


      <ul
        class="nav-links"
        :class="{ open: menuOpen }"
      >

        <li>
          <RouterLink
            to="/"
            exact-active-class="active"
            @click="closeMenu"
          >
            Home
          </RouterLink>
        </li>

        <li>
          <RouterLink
            to="/about"
            active-class="active"
            @click="closeMenu"
          >
            About
          </RouterLink>
        </li>

        <li>
          <RouterLink
            to="/skills"
            active-class="active"
            @click="closeMenu"
          >
            Skills
          </RouterLink>
        </li>

        <li>
          <RouterLink
            to="/projects"
            active-class="active"
            @click="closeMenu"
          >
            Projects
          </RouterLink>
        </li>

        <li>
          <RouterLink
            to="/contact"
            active-class="active"
            @click="closeMenu"
          >
            Contact
          </RouterLink>
        </li>

      </ul>

    </nav>

  </header>

</template>