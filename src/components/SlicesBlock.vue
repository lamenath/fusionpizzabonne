<template>
    <div class="container">
        <!-- Slice section template -->
        <section v-for="(slice, index) in slices" :key="'slice-' + index">
            <!-- Text slice component -->
            <template v-if="slice.slice_type === 'text_section'">
                <text-slice :slice="slice"/>
            </template>
            <!-- Credits slice component -->
            <template v-if="slice.slice_type === 'credits_section'">
                <text-slice :slice="slice"/>
            </template>
            <!-- Full Width Image slice component -->
            <template v-else-if="slice.slice_type === 'full_width_image'">
                <full-width-image :slice="slice"/>
            </template>
            <!-- Buttons slice component -->
            <template v-else-if="slice.slice_type === 'buttons'">
                <buttons :slice="slice"/>
            </template>
            <!-- Record slice component -->
            <template v-else-if="slice.slice_type === 'record'">
                <record :slice="slice"/>
            </template>
        </section>
    </div>
</template>

<script>
// Imports for all slices
const TextSlice = () => import("./slices/TextSlice.vue");
const CreditsSlice = () => import("./slices/CreditsSlice.vue");
const FullWidthImage = () => import("./slices/FullWidthImage.vue");
const Buttons = () => import("./slices/Buttons.vue");
const Record = () => import("./slices/Record.vue");

export default {
  props: ['slices'],
  name: 'slices-block',
  components: {
    TextSlice,
    CreditsSlice,
    FullWidthImage,
    Buttons,
    Record
  },
}
</script>