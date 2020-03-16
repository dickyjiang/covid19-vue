<template>
  <div id="app" class="max-h-screen flex flex-col">
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

    <div class="flex flex-1 bg-gray-700 justify-between">
      <!-- sidepanel left -->
      <div class="w-64 bg-beige pl-2 pr-12">
        <div
          class="text-4xl font-extrabold text-bg-gray-700 text-left leading-10 pt-4 mt-4"
        >
          BERSAMA
          <div class="block">
            KITA
          </div>
          BISA
        </div>
        <div
          style="font-family:'Shrikhand', display;"
          class="text-left text-red-700 text-2xl"
        >
          #lawancorona
        </div>
        <div class="flex flex-col items-start">
          <div class="text-base font-bold text-gray-700 mt-4">
            Cari Lokasi
          </div>
          <input
            class="w-54 p-2 rounded-md mt-2"
            type="search"
            name="lokasi"
            id="lokasi"
          />
        </div>
      </div>

      <!-- middle section -->
      <div class="flex flex-col w-3/4 justify-between">
        <!-- map section   -->
        <div>
          <div class="object-contain w-full container mx-auto">
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
                    style="border: none"
                /></a> </noscript
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
        </div>
        <!-- graph section -->
        <div class="flex-initial h-64 bg-gray-600">
          graph
        </div>
      </div>

        <!-- side panel right -->
      <div class="flex flex-col w-64 bg-gray-300">
        <div class="px-1 pb-8">
          <div class="text-left font-bold text-xl mb-3 bg-gray-500 p-3">
            Data
          </div>
          <div class="mb-2">
            <div class="text-base font-bold w-full text-left mb-2">
              Provinsi
              <div class="text-lg font-semibold">
                'Data Provinsi'
              </div>
            </div>
            <div class="text-base font-bold w-full text-left mb-2">
              Kota / Kabupaten
              <div class="text-lg font-semibold">
                'Data Kota'
              </div>
            </div>
            <div class="text-base font-semibold w-full text-left mb-2">
              Kecamatan
              <div class="text-lg font-semibold">
                'Data Kecamatan'
              </div>
            </div>
            <div class="text-base font-semibold w-full text-left mb-2">
              Kelurahan / Desa
              <div class="text-lg font-semibold">
                'Data Desa'
              </div>
            </div>
          </div>

          <div class="bg-gray-500 mt-2">
            <div class="text-base font-semibold w-full text-left">
              Status
            </div>
            <div class="text-base font-semibold w-full text-left">
              Gender
            </div>
            <div class="text-base font-semibold w-full text-left">
              Usia
            </div>
          </div>
        </div>

        <div class="flex-1 bg-gray-900">
          <div class="w-full mt-2 p-2">
            <header
              class="text-lg text-white text-left font-semibold pb-2 mb-2 border-b bordeer-gray-100"
            >
              Latest Tweet
            </header>

            <div class=" h-full overflow-y-scroll">
              <div
                class="mt-3 border px-3 py-5 bg-gray-800 rounded-md shadow-md flex flex-start"
              >
                <div
                  class="rounded-full bg-gray-200 h-10 w-10 mr-4 flex-shrink-0"
                >
                  pic
                </div>
                <div class="flex flex-col flex-1 items-start">
                  <div class="text-gray-200 font-bold text-left text-xl">
                    Twitter account
                  </div>
                  <p class="text-gray-300 text-xl mb-2 leading-tight truncate">
                    sample of long tweets form user
                  </p>
                  <p
                    class="text-gray-400 fonts-base leading-tight break-all text-left"
                  >
                    #lawancorona #covid19 #corona
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "app",
  mounted() {
    var divElement = document.getElementById("viz1584294563043");
    var vizElement = divElement.getElementsByTagName("object")[0];
    if (divElement.offsetWidth > 800) {
      vizElement.style.width = "1366px";
      vizElement.style.height = "1366px";
    } else if (divElement.offsetWidth > 500) {
      vizElement.style.width = "100%";
      vizElement.style.height = "1200px";
    } else {
      vizElement.style.width = "100%";
      vizElement.style.height = "1200px";
    }
    var scriptElement = document.createElement("script");
    scriptElement.src = "https://public.tableau.com/javascripts/api/viz_v1.js";
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
  }
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
