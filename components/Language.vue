<template>
  <div class="flex flex-row text-[12px] gap-2 my-[2px]">
    <div class="flex flex-col justify-center">
      <img :src="icon" height="10px" width="10px" />
    </div>
    <div class="text-highlight font-bold text-code">
      {{ name }}
    </div>
    <div class="flex-grow text-right italic">{{ level }}</div>
    <div class="flex flex-row gap-[1px] items-end pb-[1px] text-[10px]">
      <span
        v-for="i in 5"
        :key="i"
        :style="{ color: parseInt(points || '1') >= i ? '#2563eb' : '#bfdbfe' }"
      >
        <i class="fa fa-circle" aria-hidden="true"></i>
      </span>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps({
  icon: String,
  name: String,
  level: String,
  points: String,
});
</script>
