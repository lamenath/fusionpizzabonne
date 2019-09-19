<template>
  <section class='buttons'>
	    <prismic-rich-text :field="slice.primary.label"/>
  </section>
</template>

<script>
export default {
  props: ['slice'],
  name: 'buttons'
}
</script>

<style>
.buttons {
width: 30%;
height: 100%;
background-color: transparent;
border: 10px solid white;
border-radius: 3px;
text-align: center;
-webkit-transition-duration: 0.2s; /* Safari */
transition-duration: 0.2s;
}
.buttons:hover {
  background-color: white;
}

</style>