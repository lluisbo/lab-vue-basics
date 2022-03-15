<template>
  <div class="home">
     <Navbar />
    <p v-html="sum"></p>
    <img v-if="showElement" alt="Vue logo" src="../assets/logo.png">
    <ButtonToggle />
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import ButtonToggle from "@/components/ButtonToggle.vue"

export default {
  name: 'HomeView',
  components: {
   Navbar,
   Footer,
   ButtonToggle,
  },
  data() {
    return {
        sum: 2 + 2,
        showElement: false,
    }
  },
}
</script>
