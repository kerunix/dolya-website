<template>
  <div class="py-20 w-full md:w-1/2 flex flex-col space-y-16 px-10">
    <h1 class="font-bold text-xl md:text-3xl text-center md:text-left text-pink-600 uppercase tracking-widest">
      Videos
    </h1>
    <div class="flex flex-col md:flex-row justify-around space-y-16 md:space-y-0 md:space-x-16">
      <TheYoutube video-id="CBDYlllY1Zo" />
      <TheYoutube video-id="U0HimHlz_-c" />
    </div>
  </div>
</template>

<script>
import TheYoutube from '~/components/common/TheYoutube'

export default {
  components: {
    TheYoutube
  }
}
</script>
