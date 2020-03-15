<template>
  <div id="app">
    <header
      class="flex justify-between items-end bg-white py-3 px-2 md:px-12 shadow-lg"
    >
      <div>
        <h3
          class="text-md md:text-xl font-black tracking-tight leading-none text-gray-700 text-left"
        >
          Novel
          <span class="block">
            Coronavirus
          </span>
          <span class="block text-md md:text-lg font-light">
            COVID-19
          </span>
        </h3>
      </div>
      <div>
        <div class="hidden md:block text-base text-gray-600 font-semibold">
          <button class="mx-4">
            Halaman Depan
          </button>
          <button class="mx-4">
            Informasi
          </button>
          <button class="mx-4">
            Tentang Kami
          </button>
        </div>
      </div>
    </header>

    <div class="flex-1 bg-gray-200 container mx-auto pt-8 min-w-full h-screen">
      <div
        class="relative max-w-screen-lg h-3/4 container mx-auto object-contain pt-24 pb-12 px-12"
      >
        
        <div class="absolute top-0 left-0 pt-2 md:pt-4 pl-8 md:pl-8">
          <h1
            style="font-family:'Shrikhand', display;"
            class="text-2xl md:text-5xl text-left leading-none"
          >
            Bersama Kita Bisa !
            <span class="block text-left text-red-700 text-xl md:text-4xl">
              #lawancorona
            </span>
          </h1>
        </div>
      </div>
      <div
        class="container mx-auto w-full h-auto md:w-3/4 py-2"
      >
        <div
          class="tableauPlaceholder"
          id="viz1584294563043"
          style="position: relative; max-width: 100%;"
        >
          <noscript
            ><a href="#"
              ><img
                alt=" "
                src="https://public.tableau.com/static/images/Pe/PetaSebaranODPPDP-BlueVersion/DashboardMapAllCases/1_rss.png"
                style="border: none"/></a></noscript
          ><object class="tableauViz" style="display:none;"
            ><param name="host_url" value="https://public.tableau.com/"/>
            <param name="embed_code_version" value="3"/>
            <param
              name="path"
              value="views/PetaSebaranODPPDP-BlueVersion/DashboardMapAllCases?:embed=y&amp;:display_count=y"/>
            <param name="toolbar" value="no"/><param
              name="static_image"
              value="https://public.tableau.com/static/images/Pe/PetaSebaranODPPDP-BlueVersion/DashboardMapAllCases/1.png"/>
            <param name="animate_transition" value="yes"/><param
              name="display_static_image"
              value="yes"/><param name="display_spinner" value="yes"/><param
              name="display_overlay"
              value="yes"/><param name="display_count" value="yes"
          /></object>
        </div>
      </div>
      <div
        class="container mx-auto bg-white h-48 w-4/5 md:w-3/4 rounded-lg shadow-xl py-2 px-4"
      >
        <div class="text-2xl font-black text-center pt-4 pb-8">
        Cari Lokasi Rumah Sakit Rujukan Terdekat
        </div>
        <div class="flex justify-around items-center">
          <div class="flex-initial font-semibold text-white bg-red-700 w-1/4 py-3 px-3 m-1 rounded-lg shadow-md">
          Provinsi
          </div>
          <div class="flex-initial font-semibold text-white bg-red-700 w-1/4 py-3 px-3 m-1 rounded-lg shadow-md">
          Kota / Kabupaten
          </div>
          <div class="flex-initial font-semibold text-white bg-red-700 w-1/4 py-3 px-3 m-1 rounded-lg shadow-md">
          Kecamatan
          </div>
          <div class="flex-initial font-semibold text-white bg-red-700 w-1/4 py-3 px-3 m-1 rounded-lg shadow-md">
          Kelurahan / Desa
          </div>
        </div>
      </div>

      <div
        class="flex container mx-auto w-3/4 justify-evenly flex-stretch mt-12 "
      >
        <div class=" w-2/6 ">
          <H2
            style="font-family:'Barlow Condensed', sans-serif;"
            class="m-2 text-xl font-bold text-left"
          >
            Apa itu corona virus ?
          </H2>
          <p class="text-left pr-8 border-r-2 border-gray-400">
            Coronavirus merupakan keluarga besar virus yang menyebabkan penyakit
            ringan sampai berat, seperti common cold atau pilek dan penyakit
            yang serius seperti MERS dan SARS - Penularannya dari hewan ke
            manusia (zoonosis) dan penularan dari manusia ke manusia sangat
            terbatas.
          </p>
        </div>
        <div class="w-2/6">
          col 2
        </div>
        <div class="w-2/6 bg-gray-400">
          Twitter column
        </div>
      </div>
    </div>

    <!-- <div class="h-screen bg-blue-200">
      section 2
    </div> -->
  </div>
</template>

<script>
export default {
  name: 'app',
  mounted () {
    var divElement = document.getElementById('viz1584294563043');
    var vizElement = divElement.getElementsByTagName('object')[0];
    if (divElement.offsetWidth > 800) {
      vizElement.style.width = '1366px';
      vizElement.style.height = '1366px';
    } else if (divElement.offsetWidth > 500) {
      vizElement.style.width = '100%';
      vizElement.style.height = '1200px';
    } else {
      vizElement.style.width = '100%';
      vizElement.style.height = '1200px';
    }
    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
  },
};
</script>

<style>
#app {
  font-family: Barlow, Shrikhand, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
