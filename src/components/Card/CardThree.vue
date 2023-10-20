<script setup>
const items = [
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/227-403/marketingbillboard_20230221215933.jpeg/format:webp",
    title: "Deprem bölgelerine destek olabilirsiniz",
    url: "https://www.hepsiburada.com/kampanyalar/deprem-yardim-kartlari",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/227-403/marketingbillboard_20230912110951.png/format:webp",
    title: "Kolay yolculuk",
    url: "https://www.hepsiburadaseyahat.com/?utm_source=hepsiburada&utm_medium=web&utm_campaign=billboard_hepsiburada_web",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/227-403/marketingbillboard_20230912111117.jpeg/format:webp",
    title: "3 saatte bir yenilenen fırsatlar",
    url: "https://www.hepsiburada.com/dort-dortluk-kampanya",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/227-403/marketingbillboard_20230920163105.jpeg/format:webp",
    title: "Hepsipay ile tanış",
    url: "https://giris.hepsiburada.com/?ReturnUrl=https%3A%2F%2Foauth.hepsiburada.com%2Fconnect%2Fauthorize%2Fcallback%3Fclient_id%3DSPA%26redirect_uri%3Dhttps%253A%252F%252Fwww.hepsiburada.com%252Fuyelik%252Fcallback%26response_type%3Dcode%26scope%3Dopenid%2520profile%26state%3De24740663b8b4967a2397c142c6f0167%26code_challenge%3DX_-IJiVn7iCZD5eV6PZT8ishIjZ2hyqLIB0r0nEHd_8%26code_challenge_method%3DS256%26response_mode%3Dquery%26ActivePage%3DPURE_LOGIN%26oidcReturnUrl%3Dhttps%253A%252F%252Fwww.hepsiburada.com%252Fcuzdanim%252F",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/227-403/marketingbillboard_20230912111000.png/format:webp",
    title: "Süper fiyatlarla yurt dışından ürünler",
    url: "https://www.hepsiburada.com/kampanyalar/yurt-disindan-urunler?wt_int=hybanner.yurtdisi.kampanya",
  },
];
</script>

<template>
  <div class="flex justify-evenly items-center">
    <div
      class="flex flex-col justify-center items-center w-full"
      v-for="item in items"
      :key="item"
    >
      <h1 class="font-bold text-xl text-gray-600">{{ item.title }}</h1>
      <img :src="item.image" alt="" class="w-56 mt-4 rounded" />
    </div>
  </div>
</template>
