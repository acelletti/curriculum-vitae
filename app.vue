<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<script setup lang="ts">
useSeoMeta({
  title: "Curriculum Vitae",
  description:
    "A motivated, adaptable and responsible Software Engineer with strong experience as a Team Leader and a proven track record for innovation and critical thinking.",

  // OG tags
  ogUrl: "https://acelletti.github.io/curriculum-vitae/",
  ogTitle: "Andrea Celletti's Curriculum Vitae",
  ogDescription: "Staff Software Engineer at Vonage.",
  ogImage: "https://acelletti.github.io/curriculum-vitae/img/ogCard.png",

  // twitter tags
  twitterCard: "summary_large_image",
  twitterTitle: "Andrea Celletti's Curriculum Vitae",
  twitterDescription: "Staff Software Engineer at Vonage.",
  twitterImage: "https://acelletti.github.io/curriculum-vitae/img/ogCard.png",
});
</script>
