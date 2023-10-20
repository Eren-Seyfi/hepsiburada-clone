<script setup>
const props = defineProps(["data"]);
</script>
<template>
  <div
    class="flex flex-col items-center justify-evenly border-2 h-full rounded group w-56"
  >
    <span class="text-center text-xs truncate w-full px-2">{{ props.data.title }}</span>
    <img class="h-3/5" :src="props.data.image" alt="" />

    <span
      class="group-hover:hidden text-xl font-bold text-orange-500 w-36 h-10 text-center"
      >{{ props.data.price }} TL</span
    >
    <a :href="props.data.url"
      class="group-hover:block hidden text-orange-600 font-bold text-xl text-center rounded bg-orange-100 hover:bg-orange-200 w-36 h-10"
    >
      Sepete Ekle
    </a>
  </div>
</template>
