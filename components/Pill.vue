<script setup lang="ts">
defineProps<{ accent?: 'go' | 'warn' | 'stop' }>()
</script>

<template>
  <span :class="['pill', accent ? `accent-${accent}` : '']"><slot /></span>
</template>
