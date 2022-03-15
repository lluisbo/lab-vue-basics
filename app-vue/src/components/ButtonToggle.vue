<template>
<div>
     <button @click="toggleButton">Click me</button>
</div>
  
</template>

<script>
export default {
 data() {
    return {
        showElement: false,
    }
  },
  methods: {
        toggleButton() {
           if(!this.showElement) {
             this.showElement = true;
           } else {
             this.showElement = false;
           }
        },
      
    }
}
</script>

<style>

</style>