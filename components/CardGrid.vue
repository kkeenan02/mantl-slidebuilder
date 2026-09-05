<script setup lang="ts">
defineProps<{ cols?: 2 | 3 }>()
</script>

<template>
  <div :class="cols === 2 ? 'card-grid-2' : 'card-grid-3'">
    <slot />
  </div>
</template>
