<template>
  <div class="home">
     <Navbar />
    <p v-html="sum"></p>
    <img v-if="showElement" alt="Vue logo" src="../assets/logo.png">
<<<<<<< Updated upstream
    <ButtonToggle>CLICK ME</ButtonToggle>
=======
    <ButtonComponent>CLICKE ME</ButtonComponent>
>>>>>>> Stashed changes
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import ButtonComponent from "@/components/ButtonComponent.vue"

export default {
  name: 'HomeView',
  components: {
   Navbar,
   Footer,
   ButtonComponent,
  },
  data() {
    return {
        sum: 2 + 2,
        showElement: false,
    }
  },
}
</script>
