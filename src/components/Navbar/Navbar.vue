<script setup>
import Top from "./Top.vue";
import Middle from "./Middle.vue";
import Bottom from "./Bottom.vue";
</script>
<template>
  <div class="my-3 space-y-4">
    <Top class="px-40" />
    <Middle class="px-40" />
    <div class="flex">
      <div class="bg-orange-500 w-7/12 h-2"></div>
      <div class="bg-blue-500 w-1/6 h-2"></div>
      <div class="bg-purple-500 w-1/6 h-2"></div>
      <div class="bg-green-500 w-1/6 h-2"></div>
      <div class="bg-fuchsia-950 w-1/6 h-2"></div>
    </div>

    <Bottom class="px-40" />
  </div>
</template>
