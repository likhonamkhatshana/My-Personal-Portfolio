<script setup>
import { socialLinks } from '../data/portfolio.js'

defineProps({
  compact: {
    type: Boolean,
    default: false,
  },
})
</script>

<template>

  <div
    class="social-links"
    :class="{ compact }"
  >

    <a
      v-for="social in socialLinks"
      :key="social.name"

      :href="social.url"

      :aria-label="social.name"
      :title="social.name"

      :target="
        social.name === 'Email'
          ? undefined
          : '_blank'
      "

      :rel="
        social.name === 'Email'
          ? undefined
          : 'noopener noreferrer'
      "
    >

      <span>
        {{ social.icon }}
      </span>

      <span v-if="!compact">
        {{ social.name }}
      </span>

    </a>

  </div>

</template>