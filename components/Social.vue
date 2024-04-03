<template>
<div class="flex flex-col gap-2 mb-[10px]">
  <div class="flex flex-row items-center gap-2 italic text-[14px]">
    <i class="fa fa-github text-[16px]"></i>
    <a :href="github" target="_blank" rel="noopener noreferrer">{{ removeHttps(github) }}</a>
  </div>
  <div class="flex flex-row items-center gap-2 italic text-[14px]">
    <i class="fa fa-linkedin-square text-[16px] text-[#0077B5]"></i>
    <a :href="linkedin" target="_blank" rel="noopener noreferrer">{{ removeHttps(linkedin) }}</a>
  </div>
</div>
</template>

<script setup lang="ts">
defineProps({
  github: String,
  linkedin: String,
})

const removeHttps = (url: string) => url.replace(/^https:\/\/(www.)?/, '');
</script>