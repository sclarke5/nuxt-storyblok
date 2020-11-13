<template>
  <div
    v-editable="blok"
    class="prose my-24 mx-auto">
    <h1>{{ blok.name }}</h1>
    <img 
      class="h-200 w-200"
      :src="blok.hero" />
    <h3 class="text-blue-500"> {{ blok.intro }} </h3>
    <rich-text-renderer 
      :document="blok.body"
    />
    
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