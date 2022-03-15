<template>
<div>
   <Navbar />
  <img alt="Vue logo" src="../assets/logo.png">
  <Post />
  <Footer />
</div>
</template>

<script>
import Footer from "@/components/Footer.vue";
import Navbar from "@/components/Navbar.vue";
import Post from "@/components/Post.vue";

export default {
 name: "AboutView",
 components: {
   Navbar,
   Footer,
   Post,
 },
}
</script>

<style>

</style>

