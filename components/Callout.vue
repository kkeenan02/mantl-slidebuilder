<script setup lang="ts">
const props = defineProps<{
  /** accent border/background: teal (default) | go | warn | stop | neutral */
  accent?: 'teal' | 'go' | 'warn' | 'stop' | 'neutral'
}>()

const map: Record<string, [string, string]> = {
  teal:    ['rgba(20,184,166,.5)',  'rgba(20,184,166,.10)'],
  go:      ['rgba(16,185,129,.5)',  'rgba(16,185,129,.10)'],
  warn:    ['rgba(245,158,11,.5)',  'rgba(245,158,11,.10)'],
  stop:    ['rgba(244,63,94,.5)',   'rgba(244,63,94,.10)'],
  neutral: ['rgba(56,189,248,.5)',  'rgba(56,189,248,.10)'],
}

const style = props.accent && props.accent !== 'teal'
  ? { borderColor: map[props.accent][0], background: map[props.accent][1] }
  : {}
</script>

<template>
  <div class="callout" :style="style">
    <slot />
  </div>
</template>
