<template>
  <a class="button" :href="slice.primary.link.url">{{slice.primary.label}}</a>
</template>

<script>
export default {
  props: ['slice'],
  name: 'buttons'
}
</script>

<style scoped="true">
.button {
width: 30%;
height: 100%;
background-color: transparent;
border: 1px solid white;
border-radius: 2px;
text-align: center;
-webkit-transition-duration: 0.2s; /* Safari */
transition-duration: 0.2s;
color: white;
font-size: 24px;
padding: 10px 10px 10px 10px;
margin-left: 40%;
}
.button:hover {
  background-color: white;
  color:black;
}

</style>