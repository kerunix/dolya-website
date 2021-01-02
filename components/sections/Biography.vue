<template>
  <div class="py-20 w-full md:w-1/2 flex flex-col space-y-16 px-10">
    <h1 class="font-bold text-xl md:text-3xl text-center md:text-left uppercase tracking-widest text-teal-300">
      {{ $t('biography.about') }}
    </h1>
    <div class="flex flex-col md:flex-row md:justify-around md:space-x-16 space-y-8 md:space-y-0">
      <img src="~/assets/img/dolya.jpg" alt="A picture of the band" class="md:w-1/3">
      <div class="text-lg">
        {{ $t('biography.one') }}
      </div>
    </div>
    <div class="flex flex-col md:flex-row md:justify-around md:space-x-16 space-y-8 md:space-y-0">
      <div class="text-lg">
        {{ $t('biography.two') }}
      </div>
      <img src="~/assets/img/dolya-2.jpg" alt="A picture of the band" class="md:w-1/3">
    </div>
  </div>
</template>

<script>
export default {

}
</script>
