<template>
  <div id="home" class="bg-black text-gray-200">
    <TheNavbar />
    <TheHero />
    <TheSection>
      <NewEP />
    </TheSection>
    <TheSection id="bio">
      <Biography />
    </TheSection>
    <TheSection id="videos">
      <Videos />
    </TheSection>
    <TheSection id="contact">
      <Contact />
    </TheSection>
    <TheFooter />
  </div>
</template>

<script>
import TheNavbar from '~/components/navigation/TheNavbar'
import TheHero from '~/components/layout/TheHero'
import TheSection from '~/components/layout/TheSection'
import NewEP from '~/components/sections/NewEP'
import Biography from '~/components/sections/Biography'
import Videos from '~/components/sections/Videos'
import Contact from '~/components/sections/Contact'
import TheFooter from '~/components/layout/TheFooter'

export default {
  components: {
    TheNavbar,
    TheSection,
    TheHero,
    NewEP,
    Biography,
    Videos,
    Contact,
    TheFooter
  }
}
</script>

<style>
html {
  scroll-behavior: smooth;
}
</style>
