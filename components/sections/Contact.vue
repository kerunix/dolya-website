<template>
  <div class="py-20 w-full md:w-1/2 flex flex-col justify-center items-center space-y-10 px-10">
    <h1 class="font-bold text-xl md:text-3xl text-center md:text-left uppercase tracking-widest text-teal-300 mb-6">
      Booking/Managment
    </h1>
    <span> +33 674 595 011</span>
    <a href="mailto:contact.dolya@gmail.com" class="hover:text-teal-300">contact.dolya@gmail.com</a>
    <div class="flex space-x-10 text-gray-200">
      <a href="https://www.instagram.com/dolyaband/" target="_blank" class="text-white">
        <InstagramIcon />
      </a>
      <a href="https://www.facebook.com/dolyaofficiel" target="_blank" class="text-white">
        <FacebookIcon />
      </a>
    </div>
  </div>
</template>

<script>
import InstagramIcon from '~/components/icons/InstagramIcon'
import FacebookIcon from '~/components/icons/FacebookIcon'
export default {
  components: {
    InstagramIcon,
    FacebookIcon
  }
}
</script>
