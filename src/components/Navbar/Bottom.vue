<script setup>
const items = [
  {
    title: "Elektronik",
  },
  {
    title: "Moda",
  },
  {
    title: "Ev, Yaşam, Kırtasiye, Ofis",
  },
  {
    title: "Oto, Bahçe, Yapı Market",
  },
  {
    title: "Anne, Bebek, Oyuncak",
  },
  {
    title: "Spor, Outdoor",
  },
  {
    title: "Kozmetik, Kişisel Bakım",
  },
  {
    title: "Süpermarket, Pet Shop",
  },
  {
    title: "Kitap, Müzik, Film, Hobi",
  },
];
</script>

<template>
  <div class="flex space-x-6">
    <a
      href="#"
      class="text-center border-l border-gray-200 pl-4 text-gray-600 font-bold text-xs"
      v-for="item in items"
      :key="item"
      >{{ item.title }}</a
    >
  </div>
</template>
