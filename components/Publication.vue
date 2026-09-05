<script setup lang="ts">
defineProps<{
  /** image path, e.g. /my-cover.png (place the file in the deck folder) */
  img: string
  alt?: string
  caption?: string
  /** white plate behind the image (for dark title art on a dark theme) */
  plate?: boolean
  /** box height class, default h-40 */
  height?: string
}>()
</script>

<template>
  <div>
    <div
      :class="[height ?? 'h-40', 'flex items-center justify-center rounded-lg', plate ? 'bg-white p-3' : '']"
    >
      <img :src="img" :alt="alt" class="max-h-full max-w-full object-contain rounded" />
    </div>
    <div v-if="caption" class="text-[11px] opacity-70 mt-2">{{ caption }}</div>
  </div>
</template>
