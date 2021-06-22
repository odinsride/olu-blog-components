<template>
  <div class="py-10 text-center bg-gray-50 border-t border-green-500 border-opacity-50">
    <p class="mb-2 text-gray-700">
      <slot></slot>
    </p>
    <p class="text-sm text-gray-600" v-if="links">
      <span v-for="(link, index) in links" :key="index">
        <a :href="link.url" class="text-green-600 hover:text-green-700" :aria-label="link.label">
          {{ link.label }}
        </a>
        <span v-if="index != links.length - 1"> | </span>
      </span>
    </p>
  </div>
</template>

<script>
  export default {
    name: 'OluFooter',
    props: {
      links: {
        required: false,
        type: Array
      }
    }
  }
</script>