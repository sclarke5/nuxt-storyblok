<template>
  <div
    v-editable="blok"
    class="py-8 mb-6 text-5xl font-bold text-center">
    <!-- <h1>{{blok.title}}</h1> -->
    <img 
      class="h-60 w-screen mb-4 object-cover"
      :src="blok.image.filename" />
  </div>
</template>

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