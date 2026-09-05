<script setup lang="ts">
withDefaults(defineProps<{
  /** text shown on the right (email, role, etc.) */
  right?: string
  name?: string
  tagline?: string
  /** pin to the bottom of the slide */
  fixed?: boolean
}>(), {
  right: 'you@mantl.ie',
  name: 'MANTL',
  tagline: 'DECISION INTELLIGENCE',
  fixed: true,
})
</script>

<template>
  <div
    :class="[
      'flex items-center justify-between pt-2 text-left',
      fixed ? 'absolute bottom-6 left-14 right-14' : 'mt-6',
    ]"
    style="border-top: 1px solid rgba(217,65,65,0.4)"
  >
    <div class="flex items-center gap-3">
      <svg width="30" height="30" viewBox="0 0 60 60" fill="none">
        <polygon points="30,3 51,10.5 57,30 51,49.5 30,57 9,49.5 3,30 9,10.5" stroke="rgba(255,255,255,0.35)" stroke-width="1.5" fill="none" />
        <polygon points="30,10 45,15 50,30 45,45 30,50 15,45 10,30 15,15" stroke="rgba(217,65,65,0.5)" stroke-width="1" fill="none" />
        <circle cx="30" cy="30" r="14" fill="rgba(217,65,65,0.08)" stroke="rgba(255,255,255,0.12)" stroke-width="1" />
        <circle cx="30" cy="30" r="6.5" fill="#d94141" />
      </svg>
      <div class="flex flex-col leading-none">
        <span class="text-lg font-semibold tracking-[0.25em]">{{ name }}</span>
        <span class="text-[9px] font-medium tracking-[0.22em] mt-1" style="color:#d94141">{{ tagline }}</span>
      </div>
    </div>
    <div class="text-sm" style="color:#d94141">{{ right }}</div>
  </div>
</template>
