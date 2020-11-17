<template>
  <div
    v-editable="blok"
    class="py-8 mb-6 text-5xl font-bold text-center container">
    <!-- <h1>{{blok.title}}</h1> -->
    <img 
      class="h-60 w-screen mb-4 object-cover"
      :src="blok.image.filename" />
    <h1 class="hero-header">{{ blok.header}}</h1>
    <h2 class="hero-intro">{{ blok.intro }}</h2>
  </div>
</template>

<style>
  .hero-header {
    position: absolute;
    top: 35%;
    left: 150px;
    padding-right: 400px;
    color: white;
    font-size: 80px;
    font-family: Impact, Charcoal, sans-serif;
  }
  .hero-intro {
    position: absolute;
    top: 35%;
    right: 50px;
    padding-left: 600px;
    color: white;
    font-size: 30px;
    font-family: Impact, Charcoal, sans-serif;
  }

</style>

<script>
export default {
  props: {
    blok: {
      type: Object,
      required: true
    }
  }
}
</script>