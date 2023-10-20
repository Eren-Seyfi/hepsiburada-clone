<script setup>
const bankalar = [
  { url: "https://images.hepsiburada.net/assets/footer-sf/bonus-new.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/maximum-new.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/world-new.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/ziraat-new.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/finans-new.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/axess-new-3.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/advantage-new.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/paraf-new.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/visa.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/mastercard.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/ae.svg" },
  { url: "https://images.hepsiburada.net/assets/footer-sf/troy.svg" },
];
</script>

<template>
  <footer class="bg-zinc-200 flex justify-between space-x-20 py-2">
    <!-- ==================== Markalar ==================== -->
    <div class="w-4/12 py-4 space-y-4">
      <div class="flex flex-row h-8 space-x-3">
        <img
          src="https://images.hepsiburada.net/banners/0/imageUrl2094_20201110131516.png"
          class="w-full"
        />
        <img
          src="https://images.hepsiburada.net/banners/0/imageUrl2107_20201110131529.png"
          class="w-full"
          alt=""
        />
        <img
          src="https://images.hepsiburada.net/assets/footerWebP/imageUrl2066_20201110131447.webp"
          class="w-full"
          alt=""
        />
        <img
          src="https://images.hepsiburada.net/assets/footerWebP/imageUrl2114_20201110131437.webp"
          class="w-full"
          alt=""
        />
        <img
          src="https://images.hepsiburada.net/assets/footerWebP/imageUrl2122_20201216131442.webp"
          class="w-full"
          alt=""
        />
      </div>

      <div class="flex flex-row h-8 space-x-3">
        <img
          src="https://images.hepsiburada.net/assets/footerWebP/imageUrl2099_20201110131323.webp"
          alt=""
        />
        <img
          src="https://images.hepsiburada.net/assets/footerWebP/imageUrl2084_20201110131406.webp"
          alt=""
        />
        <img
          src="https://images.hepsiburada.net/assets/footerWebP/imageUrl2098_20201110131420.webp"
          alt=""
        />
      </div>
    </div>

    <!-- ==================== Bankalar ==================== -->
    <div class="w-8/12 space-y-4">
      <div class="flex items-center space-x-3">
        <img
          class="h-4"
          v-for="banka in bankalar"
          :src="banka.url"
          :key="banka"
          alt=""
        />
      </div>

      <div>
        <div class="text-sm">
          Her şey ayağına gelsin! © Copyright 1998 - 2023 D-MARKET Elektronik
          Hizmetler Tic. A.Ş. Her Hakkı Saklıdır.
        </div>

        <div class="text-gray-500 font-light text-xs">
          Hepsiburada.com, Bir Doğan Online Markasıdır.
        </div>
      </div>
    </div>
  </footer>
</template>
