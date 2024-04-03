<template>
  <div class="flex flex-row gap-2">
    <div class="pt-1"><span class="material-symbols-outlined text-[16px] text-highlight">{{ icon }}</span>
    </div>
    <div class="flex-grow text">
      <slot/>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps({
  icon: String,
})
</script>

<style lang="scss" scoped>
.text {
  :deep(h3) {
    color: #2563eb;
  }
}
</style>