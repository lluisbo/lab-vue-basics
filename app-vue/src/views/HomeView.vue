<template>
  <div class="home">
    <Navbar />
    <p v-html="sum"></p>
    <img v-show="showElement" alt="Vue logo" src="../assets/logo.png">
    <ButtonComponent :onClick="showOnClick">Show Vue logo</ButtonComponent>
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
  methods: {
    showOnClick(){
      if(!this.showElement) {
        this.showElement = true;
      } else {
        this.showElement = false;
      }
    }
  }
}
</script>
