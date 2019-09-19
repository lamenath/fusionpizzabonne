<template>
	<section class="record">
	</section>
</template>

<script>
export default {
  props: ['slice'],
  name: 'buttons'
}
</script>

<style>
.record {
   width: 50vw;
   height: 50vw;
   position: relative;
   overflow: hidden;
   background: url("https://prismic-io.s3.amazonaws.com/new-pizz%2F5e9963da-c1b0-428d-91d4-ce0887ffad3a_fpb.png")
   no-repeat center center;
   background-size: cover;
   animation: spin 6s linear infinite;
   margin-bottom: 50px;
   margin-left: 20%;
}

@keyframes spin {
   0% {
      transform: rotate(0deg);
   }
   100% {
      transform: rotate(360deg);
   }
}
</style>