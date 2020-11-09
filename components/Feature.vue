<template>
  <div
    v-editable="blok"
    class="py-2 grid gap-4 justify-items-center">
    <img 
      class="h-20 w-20"
      :src="blok.icon" />
    <h1 class="text-lg">{{ blok.name }}</h1>
    <p class="text-gray-500">
      {{ blok.description }}
    </p>
    <p class="text-red-700">
      {{ blok.tagline }}
    </p>
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