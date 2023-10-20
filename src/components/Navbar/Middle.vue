<template>
  <div class="flex justify-center items-center mx-4">
    <!-- ======== Logo ======== -->
    <div>
      <h1 class="font-extrabold text-4xl text-orange-500">hepsiburada</h1>
      <h3 class="font-bold text-end">
        <span class="hover:underline text-orange-500">Premium'u</span> keşfet
      </h3>
    </div>

    <!-- ======== Arama kutusu ======== -->
    <div
      class="border-gray-500 border-2 rounded-md flex w-full items-center pl-4 mx-12"
    >
      <span
        class="material-symbols-outlined text-3xl font-extrabold text-gray-500"
      >
        search
      </span>
      <input
        type="text"
        class="mx-2 border-none outline-none w-full"
        placeholder="Ürün, kategori veya marka ara"
      />
      <button
        class="bg-stone-400 text-lg font-bold uppercase text-white px-4 py-2 h-full"
      >
        ARA
      </button>
    </div>

    <!-- ======== Konum kutusu ======== -->
    <div class="flex items-center mr-6">
      <span class="material-symbols-outlined text-2xl text-orange-500">
        location_on
      </span>
      <div class="flex flex-col">
        <h3 class="font-semibold">Konum</h3>
        <p class="font-light text-sm text-orange-600">Manisa...</p>
      </div>
    </div>

    <!-- ======== Giriş yap ve Sepet kutusu ======== -->
    <div class="w-full flex items-center space-x-4 mx-2">
      <button
        class="border-2 border-gray-500 flex items-center rounded px-4 w-1/2"
      >
        <span
          class="material-symbols-outlined text-2xl font-semibold text-gray-500 my-1"
        >
          person
        </span>
        <div class="flex flex-col items-center">
          <h4 class="font-semibold">Giriş Yap</h4>
          <p class="text-sm">veya üye ol</p>
        </div>
      </button>

      <button
        class="bg-stone-500 text-white w-1/2 flex space-x-2 items-center px-2 py-3 rounded"
      >
        <span class="material-symbols-outlined font-medium">
          shopping_cart
        </span>
        <h3 class="text-xl font-semibold">Sepetim</h3>
      </button>
    </div>
  </div>
</template>
