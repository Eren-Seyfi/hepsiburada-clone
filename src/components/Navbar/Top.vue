<script setup>
const items = [
  {
    title: "Siparişlerim",
  },
  {
    title: "Süper Fiyat, Süper Teklif",
  },
  {
    title: "Yurt Dışından",
  },
  {
    title: "Kampanyalar",
  },
  {
    title: "Girişimci Kadınlar",
    color: "text-red-500",
  },
  {
    title: "Müşteri Hizmetleri",
  },
  {
    title: "Hepsiburada Premium",
    color: "text-orange-600",
  },
  {
    title: "Hepsiburada'da Satıcı Ol",
  },
];

</script>

<template>
  <div class="flex justify-end items-center">
    <a
      href="#"
      class="ml-2 text-xs text-gray-600 font-semibold"
      :class="item.color"
      v-for="item in items"
      :key="item"
      >{{ item.title }}</a
    >
  </div>
</template>
