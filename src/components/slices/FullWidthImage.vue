<template>
  <section class='full-width-image content-section'>
      <prismic-image :field="slice.primary.image"/>
  </section>
</template>

<script>
export default {
  props: ['slice'],
  name: 'image-caption-slice'
}
</script>

<style>
.full-width-image {
padding: 150px 50px 0 50px;
}
.full-width-image img {
  box-shadow: 15px 15px 30px black;
}
</style>