<script setup>
import Navbar from "./components/Navbar/Navbar.vue";
import Footer from "./components/Footer/Footer.vue";

import CardOne from "./components/Card/CardOne.vue";
import CardTwo from "./components/Card/CardTwo.vue";
import CardThree from "./components/Card/CardThree.vue";
import CardFour from "./components/Card/CardFour.vue";
import CardFive from "./components/Card/CardFive.vue";
const slideBarMenu = [
  {
    title: "Gamer Fırsaarı",
  },
  {
    title: "Kampanyalar",
  },
  {
    title: "Kaçınılmayacak Fiyaar",
  },
  {
    title: "Teknolojik Fırsaar",
  },
  {
    title: "Okul Alışverişi",
  },
  {
    title: "Sana Özel Fırsaar",
  },
  {
    title: "Ayrıcalıklar",
  },
];

const superFiyat_SuperTeklif = [
  {
    image:
      "https://productimages.hepsiburada.net/s/426/550/110000456733347.jpg/format:webp",
    price: "999,99 ",
    title:
      "Karaca Just Coffee Aroma 2 In 1 Filtre Kahve ve Çay Demleme Makinesi Rosegold",
    url: "https://www.hepsiburada.com/karaca-just-coffee-aroma-2-in-1-filtre-kahve-ve-cay-demleme-makinesi-rosegold-p-HBCV000023UZGZ?magaza=Karaca",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/375/550/110000359248504.jpg/format:webp",
    price: "339,00 ",
    title: "D'S Damat Relaxed Fit Siyah Sweatshirt 8HCE2ORT01001",
    url: "https://www.hepsiburada.com/d-s-damat-relaxed-fit-siyah-sweatshirt-8hce2ort01001-p-HBCV000027NVRZ?magaza=D%27S%20DAMAT",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/408/550/110000435856400.jpg/format:webp",
    price: "119,99",
    title: "June Fil Desenli Bebek Battaniye",
    url: "https://www.hepsiburada.com/june-fil-desenli-bebek-battaniye-p-HBCV000042N3VH?magaza=Hepsiburada",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/405/550/110000433411407.jpg/format:webp",
    price: "8.299,00 ",
    title: "Philips 7000 Serisi Airfryer Combi XXL Connected - HD9880/90",
    url: "https://www.hepsiburada.com/philips-7000-serisi-airfryer-combi-xxl-connected-hd9880-90-p-HBCV00004BGZ13?magaza=Hepsiburada",
  },
];

const HepsiburadaHerkes_İçinAyrıcalıkVar = [
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_1_20221025094000.png/format:webp",
    title: "Hepsiburada Market",
    url: "https://www.hepsiburada.com/hb-market/",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_1_20230426135117.jpeg/format:webp",
    title: "Sana Özel Fırsatlar",
    url: "https://sanaozel.hepsiburada.com/",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_1_20230725150730.png/format:webp",
    title: "Hepsiburada Seyahat",
    url: "https://www.hepsiburadaseyahat.com/",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_1_20211215191105.png/format:webp",
    title: "Hepsipay",
    url: "https://www.hepsiburada.com/staticpage/761309683226131",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_1_20211215191959.jpeg/format:webp",
    title: "Girişimci Kadınlar",
    url: "https://www.hepsiburada.com/staticpage/224306451888579",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_1_20220218135219.png/format:webp",
    title: "Eskiyi Yenile",
    url: "https://www.hepsiburada.com/staticpage/875739149079795",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_1_20211215191642.jpeg/format:webp",
    title: "Kolay İade",
    url: "https://www.hepsiburada.com/kolay-iade",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_1_20220131132941.png/format:webp",
    title: "Hepsimat",
    url: "https://www.hepsiburada.com/staticPage/13390",
  },
];

const Aradığın_Markalar = [
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_68_20220720122216.png/format:webp",
    title: "Arzum",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_68_20230301164543.jpeg/format:webp",
    title: "June",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_68_20230406160223.jpeg/format:webp",
    title: "Ayakkabı Dünyası",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_68_20220418153933.png/format:webp",
    title: "Regal",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_68_20230301164742.jpeg/format:webp",
    title: "Joyster",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_68_20230510115539.jpeg/format:webp",
    title: "English Home",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_68_20230406160401.jpeg/format:webp",
    title: "Marjin",
  },
  {
    image:
      "https://images.hepsiburada.net/banners/s/0/128-80/featurelist_68_20230510115500.jpeg/format:webp",
    title: "Emsan",
  },
];

const Dizüstü_Bilgisayar_Laptop = [
  {
    image:
      "https://productimages.hepsiburada.net/s/381/222-222/110000399232674.jpg/format:webp",
    price: "25.799,00 TL",
    title:
      "Monster Abra A5 V17.3.4 Intel Core i7 11800H 32GB RAM 1 TB SSD RTX 3050 Ti Freedos 15,6 Inç FHD 144 Hz Oyun Bilgisayarı",
    url: "https://www.hepsiburada.com/monster-abra-a5-v17-3-4-intel-core-i7-11800h-32gb-ram-1-tb-ssd-rtx-3050-ti-freedos-15-6-inc-fhd-144-hz-oyun-bilgisayari-p-hbcv0000409tnt",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/435/222-222/110000468594545.jpg/format:webp",
    price: "34.999,00 TL",
    title:
      'Monster Tulpar T5 V23.2.2 Intel Core I7 12650H 32 GB Ram 1 Tb SSD 8 GB Rtx 4060 Freedos 15,6" Fhd 144 Hz Oyun Bilgisayarı',
    url: "https://www.hepsiburada.com/monster-tulpar-t5-v23-2-2-intel-core-i7-12650h-32-gb-ram-1-tb-ssd-8-gb-rtx-4060-freedos-15-6-fhd-144-hz-oyun-bilgisayari-p-hbcv00004nbdzl",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/409/222-222/110000437458623.jpg/format:webp",
    price: "22.999,00 TL",
    title:
      'HP Victus Gaming 15-FA0011NT Intel Core i5 12450H 16GB 512GB SSD RTX3050 Freedos 15.6" FHD 144Hz Taşınabilir Bilgisayar 80D33EA',
    url: "https://www.hepsiburada.com/hp-victus-gaming-15-fa0011nt-intel-core-i5-12450h-16gb-512gb-ssd-rtx3050-freedos-15-6-fhd-144hz-tasinabilir-bilgisayar-80d33ea-p-hbcv00004crj5q",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/377/222-222/110000395335270.jpg/format:webp",
    price: "26.899,00 TL",
    title:
      'MSI THIN GF63 12VE-082XTR Intel Core i5 12450H 8GB 512GB SSD RTX4050 Freedos 15.6" FHD 144Hz Taşınabilir Bilgisayar',
    url: "https://www.hepsiburada.com/msi-thin-gf63-12ve-082xtr-intel-core-i5-12450h-8gb-512gb-ssd-rtx4050-freedos-15-6-fhd-144hz-tasinabilir-bilgisayar-p-hbcv00003ycw2q",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/407/222-222/110000434856113.jpg/format:webp",
    price: "34.799,00 TL",
    title:
      'Asus TUF Gaming A15 FA507NV-LP023 AMD Ryzen 7 7735HS 16GB 512GB SSD RTX4060 Freedos 15.6" FHD Taşınabilir Bilgisayar',
    url: "https://www.hepsiburada.com/asus-tuf-gaming-a15-fa507nv-lp023-amd-ryzen-7-7735hs-16gb-512gb-ssd-rtx4060-freedos-15-6-fhd-tasinabilir-bilgisayar-p-hbcv00004bn7ck",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/378/222-222/110000396660879.jpg/format:webp",
    price: "21.999,00 TL",
    title:
      'Huawei MateBook D16 Intel Core i7 12700H 16GB 512GB SSD Windows 11 Home 16" Taşınabilir Bilgisayar',
    url: "https://www.hepsiburada.com/huawei-matebook-d16-intel-core-i7-12700h-16gb-512gb-ssd-windows-11-home-16-tasinabilir-bilgisayar-p-hbcv00002nkf5o",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/424/222-222/110000455524119.jpg/format:webp",
    price: "28.999,00 TL",
    title:
      "Hp Victus 7P648EA 16-R0053NT Intel Core I5 13500H 16GB 512GB SSD Rtx 4050 6gb 16.1 Inç 144Hz Full Hd Freedos Taşınabilir Oyuncu Bilgisayarı",
    url: "https://www.hepsiburada.com/hp-victus-7p648ea-16-r0053nt-intel-core-i5-13500h-16gb-512gb-ssd-rtx-4050-6gb-16-1-inc-144hz-full-hd-freedos-tasinabilir-oyuncu-bilgisayari-p-hbcv00004iu681",
  },
];
const Giyim = [
  {
    image:
      "https://productimages.hepsiburada.net/s/447/222-222/110000481660535.jpg/format:webp",
    price: "349,99 TL",
    title: "Otaku Bomber Ceket",
    url: "https://www.hepsiburada.com/otaku-bomber-ceket-p-hbcv00004rxn2b",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/371/222-222/110000388942063.jpg/format:webp",
    price: "319,50 TL",
    title: "Los Ojos Kadın Siyah Yüksek Bel Jogger Eşofman Altı Joggers",
    url: "https://www.hepsiburada.com/los-ojos-kadin-siyah-yuksek-bel-jogger-esofman-alti-joggers-p-hbcv00000zuip5",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/371/222-222/110000388942099.jpg/format:webp",
    price: "319,50 TL",
    title:
      "Los Ojos Kadın Siyah Yüksek Bel Toparlayıcı Çift Cepli Ispanyol Paça Tayt Bootcut",
    url: "https://www.hepsiburada.com/los-ojos-kadin-siyah-yuksek-bel-toparlayici-cift-cepli-ispanyol-paca-tayt-bootcut-p-hbcv00000ufly7",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/398/222-222/110000422982352.jpg/format:webp",
    price: "349,99 TL",
    title: "June Cepli Pantolon",
    url: "https://www.hepsiburada.com/june-cepli-pantolon-p-hbcv000040fxhy",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/384/222-222/110000384229934.jpg/format:webp",
    price: "299,99 TL",
    title: "June Kemerli Gabardin Pantolon",
    url: "https://www.hepsiburada.com/june-kemerli-gabardin-pantolon-p-hbcv00003kk78g",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/439/222-222/110000472684780.jpg/format:webp",
    price: "359,00 TL",
    title: "Lithe Ajurlu Fırfırlı Yumuşacık Kazak",
    url: "https://www.hepsiburada.com/lithe-ajurlu-firfirli-yumusacik-kazak-p-hbcv00004orgp7",
  },
  {
    image:
      "https://productimages.hepsiburada.net/s/384/222-222/110000384229930.jpg/format:webp",
    price: "299,99 TL",
    title: "June Basic Jean Pantolon",
    url: "https://www.hepsiburada.com/june-basic-jean-pantolon-p-hbcv00003kk785",
  },
];
</script>

<template>
  <div class="">
    <Navbar />

    <!-- ============= Menü +++ Ev ve yaşam ürünlerinde fırsatları kaçırma ============= -->

    <section
      class="flex flex-col items-center py-4 bg-gradient-to-b from-orange-800 via-orange-500 to-orange-700"
    >
      <!-- ======= Menü listesi ======= -->
      <div class="flex items-center space-x-10">
        <a href="#" class="px-4 py-3 bg-white rounded-full font-bold text-sm"
          >Ay Sonu Fırsat Dolu</a
        >
        <a
          href="#"
          class="text-white font-bold text-base"
          v-for="Menu in slideBarMenu"
          :key="Menu"
          >{{ Menu.title }}</a
        >
      </div>
      <!-- ======= Kayan Menü ======= -->

      <div class="bg-white flex justify-between w-9/12 rounded my-6">
        <div class="flex flex-col items-center justify-evenly w-full">
          <!-- =========== Ev ve yaşam ürünlerinde fırsaarı kaçırma =========== -->
          <div class="flex flex-col space-y-4">
            <span class="text-gray-600 font-bold text-xl"
              >Ev ve yaşam ürünlerinde</span
            >
            <span class="text-gray-600 font-extrabold text-4xl"
              >fırsatları kaçırma</span
            >
          </div>

          <!-- =========== Alışverie Başla =========== -->
          <button
            class="px-4 py-2 bg-purple-800 text-white font-bold text-lg rounded-full"
          >
            Alışverişe başla
          </button>
        </div>
        <!-- ======= Resim ======= -->

        <img
          src="https://images.hepsiburada.net/banners/s/0/672-378/bannerImage2082_20230925190659.png/format:webp"
          alt=""
          class="m-2 rounded"
        />
      </div>
    </section>

    <!-- ============= Süper Fiyat, Süper Teklif ============= -->

    <section class="container px-40 my-14 space-y-4">
      <div class="flex items-end space-x-4">
        <h1 class="text-3xl font-extrabold text-gray-700">
          Süper Fiyat, Süper Teklif
        </h1>
        <span class="font-bold text-orange-500"
          >Tümü
          <span class="material-symbols-outlined text-xs">
            arrow_forward_ios
          </span>
        </span>
      </div>

      <div class="flex justify-center items-center space-x-4 h-96">
        <img
          src="https://images.hepsiburada.net/banners/s/0/224-371/homepageImage2099_20230911133304.png/format:webp"
          class="rounded-lg h-full"
        />
        <CardOne
          v-for="superFiyatSuperTeklif in superFiyat_SuperTeklif"
          :key="superFiyatSuperTeklif"
          :data="superFiyatSuperTeklif"
        />
      </div>
    </section>

    <CardThree class="container px-40" />

    <!-- ============= Aradığın Markalar ============= -->

    <section class="container px-40 my-14 space-y-4">
      <div class="flex items-end space-x-4">
        <h1 class="text-3xl font-extrabold text-gray-700">Aradığın Markalar</h1>
        <span class="font-bold text-orange-500"
          >Tümü
          <span class="material-symbols-outlined text-xs">
            arrow_forward_ios
          </span>
        </span>
      </div>

      <div class="flex justify-between items-center">
        <CardFour
          v-for="AradığınMarkalar in Aradığın_Markalar"
          :key="AradığınMarkalar"
          :data="AradığınMarkalar"
        />
      </div>
    </section>

    <!-- ============= Hepsiburada'da herkes için ayrıcalık var ============= -->
    <section class="container px-40 my-14 space-y-4">
      <div class="flex items-end space-x-4">
        <h1 class="text-3xl font-extrabold text-gray-700">
          Hepsiburada'da herkes için ayrıcalık var
        </h1>
        <span class="font-bold text-orange-500"
          >Tümü
          <span class="material-symbols-outlined text-xs">
            arrow_forward_ios
          </span>
        </span>
      </div>

      <div class="flex justify-between items-center">
        <CardTwo
          v-for="HepsiburadaHerkesİçinAyrıcalıkVar in HepsiburadaHerkes_İçinAyrıcalıkVar"
          :key="HepsiburadaHerkesİçinAyrıcalıkVar"
          :data="HepsiburadaHerkesİçinAyrıcalıkVar"
        />
      </div>
    </section>

    <!-- ============= Dizüstü Bilgisayar Laptop ============= -->
    <section class="container px-40 my-14 space-y-4">
      <div class="flex items-end space-x-4">
        <h1 class="text-3xl font-extrabold text-gray-700">
          Dizüstü Bilgisayar Laptop
        </h1>
        <span class="font-bold text-orange-500"
          >Tümü
          <span class="material-symbols-outlined text-xs">
            arrow_forward_ios
          </span>
        </span>
      </div>

      <div class="flex justify-evenly items-center space-x-2">
        <CardFive
          v-for="DizüstüBilgisayarLaptop in Dizüstü_Bilgisayar_Laptop"
          :key="DizüstüBilgisayarLaptop"
          :data="DizüstüBilgisayarLaptop"
        />
      </div>
    </section>

    <!-- ============= Giyim ============= -->
    <section class="container px-40 my-14 space-y-4">
      <div class="flex items-end space-x-4">
        <h1 class="text-3xl font-extrabold text-gray-700">Giyim</h1>
        <span class="font-bold text-orange-500"
          >Tümü
          <span class="material-symbols-outlined text-xs">
            arrow_forward_ios
          </span>
        </span>
      </div>

      <div class="flex justify-evenly items-center space-x-2">
        <CardFive v-for="Giy in Giyim" :key="Giy" :data="Giy" />
      </div>
    </section>

    <Footer class="container px-40 space-y-4" />
  </div>
</template>
