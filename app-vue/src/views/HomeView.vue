<template>
  <div class="home">
     <Navbar />
    <p v-html="sum"></p>
    <img v-if="showElement" alt="Vue logo" src="../assets/logo.png">
     <button @click="toggleImg">Click me to show or hide IMG</button>
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: 'HomeView',
  components: {
   Navbar,
   Footer,
  },
  data() {
    return {
        sum: 2 + 2,
        showElement: false,
    }
  },
  methods: {
        toggleImg() {
           if(!this.showElement) {
             this.showElement = true;
           } else {
             this.showElement = false;
           }
        },
      
    }
}
</script>
