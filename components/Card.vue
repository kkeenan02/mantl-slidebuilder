<script setup lang="ts">
defineProps<{
  /** accent colour: go | warn | stop | neutral */
  accent?: 'go' | 'warn' | 'stop' | 'neutral'
  /** optional bold title line */
  title?: string
  /** tighter padding for dense grids */
  compact?: boolean
}>()
</script>

<template>
  <div :class="['card', `accent-${accent ?? 'neutral'}`, { compact }]">
    <div v-if="title" class="card-title">{{ title }}</div>
    <div class="card-body"><slot /></div>
  </div>
</template>
