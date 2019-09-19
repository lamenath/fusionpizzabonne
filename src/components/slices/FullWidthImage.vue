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
padding: 0 50px 0 50px;
}
.full-width-image img {
  box-shadow: 3px 3px 6px 1px rgba(0, 0, 0, 0.4);
}
</style>