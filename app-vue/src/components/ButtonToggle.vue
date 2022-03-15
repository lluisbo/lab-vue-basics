<template>
     <button  class="button">
       <slot />
     </button>  
</template>

<script>
export default {
 
}
</script>

<style scoped>
.button {
    display: inline-block;
    margin: 0.5em 0;
    padding: 1em 2em;
    background: #42b983;
    border: 2px solid #42b983;
    border-radius: 10px;
    color: #ffffff;
    font-size: 1em;
    font-weight: 700;
    line-height: 1;
    text-decoration: none;
    text-transform: uppercase;
    cursor: pointer;
    transition: 0.3s;
}
</style>