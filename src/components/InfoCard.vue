<script setup>
const { uf } = defineProps({
  uf: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div>
    {{ uf }}
  </div>
</template>
