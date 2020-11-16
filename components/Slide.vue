<template>
  <div
    v-editable="blok"
    class="py-2 grid gap-4 justify-items-center">
    <img 
      class="h-20 w-20"
      :src="blok.image" />
    <h1 class="text-lg">{{ blok.alt }}</h1>
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