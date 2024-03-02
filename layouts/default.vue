<template>
  <div>
    <slot />
  </div>
</template>
<script setup lang="ts">
const route = useRoute();

useHead({
  title: `Objective - ${route.meta.title}`,
  meta: [{ property: "og:title", content: `Objetive - ${route.meta.title}` }],
});
</script>
