<template>
  <prismic-rich-text class="credits-section" :field="slice.primary.rich_text"/>
</template>

<script>
export default {
  props: ['slice'],
  name: 'credits-slice'
}
</script>

<style>
.credits-section p {
  color: blue;
  font-size: 50px;
}
</style>
