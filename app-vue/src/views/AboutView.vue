<template>
<div>
   <Navbar />
  <img alt="Vue logo" src="../assets/logo.png">
  <button @click="changeBackGroundColor">Click me to change BG color</button>
<div class="post" 
     v-for="post in posts" :key="post.id" 
     v-bind:style="isClicked ? { 'background-color': 'red' } : null"
     >
      <ul>
        <li>
         <h2>{{ post.title }}</h2>
         <h4>{{ post.description }}</h4>
         <p>{{ post.content }}</p>
        </li>
      </ul>
</div>
  <Footer />
</div>
</template>

<script>
import Footer from "@/components/Footer.vue";
import Navbar from "@/components/Navbar.vue";
export default {
 name: "AboutView",
 components: {
   Navbar,
   Footer,
 },
 data() {
   return {
      posts: [ 
     {
     id: 1,
     title: "Headeline of the Post1",
     description: "this is a description of a Post",
     content: "Then switching the loginType in the code above will not erase what the user has already entered. Since both templates use the same elements, the <input> is not replaced - just its placeholder."
     },

     {
     id: 2,
     title: "Headeline of the Post2",
     description: "this is a description of a Post",
     content: "Then switching the loginType in the code above will not erase what the user has already entered. Since both templates use the same elements, the <input> is not replaced - just its placeholder."
    
     },
      {
     id: 3,
     title: "Headeline of the Post3",
     description: "this is a description of a Post",
     content: "Then switching the loginType in the code above will not erase what the user has already entered. Since both templates use the same elements, the <input> is not replaced - just its placeholder."
    },
   ],
   isClicked: false,
  }
},
methods: {
      changeBackGroundColor() {
      this.isClicked = !this.isClicked;
       }
     },
}
</script>

<style>

</style>

