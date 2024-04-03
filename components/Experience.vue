<template>
  <div class="flex flex-col">
    <div class="flex flex-col py-2 text-[12px]">
      <div class="flex flex-row">
        <div class="font-semibold text-highlight text-[14px]">
          {{ position }}
        </div>
      </div>
      <div class="flex flex-col mt-2 gap-[2px]">
        <div class="flex" :class="short ? 'flex-col' : 'flex-row'">
          <div class="font-semibold">{{ employer }}</div>
          <div class="flex-grow" />
          <div class="flex flex-row items-center gap-1 italic text-[12px]">
            <span class="material-symbols-outlined mt-[-1px]"
              >calendar_today</span
            >
            <span>{{ time }}</span>
          </div>
        </div>
        <div class="flex flex-row items-center gap-1 italic text-[10px]">
          <span class="material-symbols-outlined mt-[-2px]">location_on</span>
          <span>{{ loc }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps({
  position: String,
  employer: String,
  loc: String,
  time: String,
  short: { type: Boolean, default: false },
});
</script>

<style lang="scss" scoped>
.material-symbols-outlined {
  font-size: 12px;
}
</style>
