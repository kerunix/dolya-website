<template>
  <nav class="flex items-center justify-center bg-black border-t-2 border-pink-600 fixed w-full z-10">
    <ul class="flex p-4 justify-around text-gray-200 w-1/2 h-full">
      <TheNavlink to="#home">
        home
      </TheNavlink>
      <TheNavlink to="#bio">
        bio
      </TheNavlink>
      <TheNavlink to="#videos">
        videos
      </TheNavlink>
      <TheNavlink to="#contact">
        contact
      </TheNavlink>
    </ul>
  </nav>
</template>

<script>
import TheNavlink from '~/components/navigation/TheNavlink'

export default {
  components: {
    TheNavlink
  }
}
</script>

<style>

</style>
