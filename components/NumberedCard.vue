<script setup lang="ts">
const props = defineProps<{
  accent?: 'go' | 'warn' | 'stop' | 'neutral'
  /** number or short label shown in the badge */
  n?: string | number
  title?: string
  compact?: boolean
}>()

const palette: Record<string, [string, string, string]> = {
  go:      ['#34d399', 'rgba(16,185,129,.15)', 'rgba(16,185,129,.45)'],
  warn:    ['#fbbf24', 'rgba(245,158,11,.15)', 'rgba(245,158,11,.45)'],
  stop:    ['#fb7185', 'rgba(244,63,94,.15)',  'rgba(244,63,94,.45)'],
  neutral: ['#7dd3fc', 'rgba(56,189,248,.15)', 'rgba(56,189,248,.45)'],
}
const c = palette[props.accent ?? 'neutral']
const badgeStyle = { color: c[0], background: c[1], borderColor: c[2] }
</script>

<template>
  <div :class="['card', `accent-${accent ?? 'neutral'}`, { compact }]">
    <div class="flex items-center gap-2 mb-1">
      <span class="step-badge" :style="badgeStyle">{{ n }}</span>
      <span class="card-title !mb-0">{{ title }}</span>
    </div>
    <div class="card-body"><slot /></div>
  </div>
</template>
