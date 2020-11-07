<template>
  <li>
    <nuxt-link class="md:text-xl h-full p-2 md:p-4 tracking-widest uppercase hover:text-pink-600 md:border-b-2 border-black hover:border-teal-300" :to="{path: '/', hash: to}">
      <slot />
    </nuxt-link>
  </li>
</template>

<script>
export default {
  props: {
    to: {
      type: String,
      required: true
    }
  }
}
</script>
