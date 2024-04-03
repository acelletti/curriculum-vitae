<template>
  <div class="flex flex-col gap-2">
    <div class="flex flex-row items-center gap-2 italic text-[14px]">
      <span
        class="material-symbols-outlined mt-[-2px] text-[16px] text-highlight"
        >location_on</span
      >
      <span v-html="address"></span>
    </div>
    <div class="flex flex-row items-center gap-2 italic text-[14px]">
      <span
        class="material-symbols-outlined mt-[-2px] text-[16px] text-highlight"
        >call</span
      >
      <span v-html="phone"></span>
    </div>
    <div class="flex flex-row items-center gap-2 italic text-[14px]">
      <span
        class="material-symbols-outlined mt-[-1px] text-[16px] text-highlight"
        >alternate_email</span
      >
      <a :href="`mailto:email`">{{ email }}</a>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps({
  address: String,
  phone: String,
  email: String,
});
</script>
