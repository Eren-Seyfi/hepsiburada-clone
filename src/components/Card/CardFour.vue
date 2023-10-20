<script setup>
const props = defineProps(["data"]);
</script>
<template>
  <div
    class="flex flex-col justify-center items-center w-40 hover:scale-110 duration-150"
  >
    <img class="rounded w-32 border" :src="props.data.image" alt="" />

    <span class="text-center text-sm font-semibold">{{
      props.data.title
    }}</span>
  </div>
</template>
