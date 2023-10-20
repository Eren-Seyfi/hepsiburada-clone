<script setup>
const props = defineProps(["data"]);
</script>

<template>
  <a
    :href="props.data.url"
    class="group border-2 h-[270px] w-40 rounded-xl hover:scale-105 duration-150 border-gray-200"
  >
    <img :src="props.data.image" alt="" />
    <p class="truncate m-2">{{ props.data.title }}</p>
    <span class="mx-2 font-bold">{{ props.data.price }}</span>
   <div class="px-2 ">
    <button class="bg-orange-600 hidden group-hover:block hover:bg-orange-700 rounded-md  w-full text-white text-lg py-1 font-bold">
        Sepete Ekle
      </button>
   </div>
  </a>
</template>
