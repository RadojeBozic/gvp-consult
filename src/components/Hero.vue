<script setup>
import heroImage from '../assets/images/supermarkt.jpg'
import { ShieldCheck, FileCheck2 } from '@lucide/vue'

const tickerItems = [
  'Ambalaža za hranu',
  'Kozmetički proizvodi',
  'Predmeti opšte upotrebe',
  'DoC i PIF dokumentacija',
  'Procena rizika i regulatorne usklađenosti proizvoda',
  'Provera dokumentacije i komunikacija sa laboratorijama'
]
</script>

<template>
  <section id="home" class="bg-[#f8f5f1] overflow-hidden">
    <div
      class="max-w-7xl mx-auto px-6 pt-10 pb-8 lg:pt-12 lg:pb-10 grid lg:grid-cols-2 gap-10 lg:gap-14 items-center"
    >
      <div>
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          GVP Consult
        </span>

        <h1
          class="text-4xl md:text-5xl xl:text-[54px] font-serif font-bold leading-[1.08] mt-4 mb-6 text-[#222222]"
        >
          Konsultantske usluge za bezbednost proizvoda
        </h1>

        <p class="text-gray-700 text-lg leading-relaxed mb-7 max-w-2xl">
          Stručna podrška proizvođačima, uvoznicima, distributerima i
          laboratorijama u oblasti predmeta opšte upotrebe, ambalaže za hranu,
          kozmetike, igračaka i proizvoda koji dolaze u kontakt sa kožom i
          sluzokožom.
        </p>

        <div class="grid sm:grid-cols-2 gap-4 mb-8 max-w-2xl">
          <div class="flex items-start gap-3">
            <ShieldCheck class="w-6 h-6 text-orange-500 mt-1 shrink-0" />
            <p class="text-gray-700">
              Procena rizika i regulatorne usklađenosti proizvoda
            </p>
          </div>

          <div class="flex items-start gap-3">
            <FileCheck2 class="w-6 h-6 text-orange-500 mt-1 shrink-0" />
            <p class="text-gray-700">
              Provera dokumentacije i komunikacija sa laboratorijama
            </p>
          </div>
        </div>

        <div class="flex flex-wrap gap-4">
          <a
            href="#services"
            class="bg-orange-500 text-white px-7 py-3 rounded hover:bg-orange-600 transition"
          >
            Pogledajte usluge
          </a>

          <a
            href="#contact"
            class="border border-gray-700 px-7 py-3 rounded hover:bg-gray-900 hover:text-white transition"
          >
            Kontaktirajte nas
          </a>
        </div>
      </div>

      <div>
        <img
          :src="heroImage"
          alt="Proizvodi na tržištu i bezbednost ambalaže"
          class="rounded-xl shadow-2xl w-full h-[300px] md:h-[360px] lg:h-[380px] object-cover"
        />
      </div>
    </div>

    <div class="border-y border-orange-100 bg-white/80">
      <div class="ticker py-4">
        <div class="ticker-track">
          <span
            v-for="item in tickerItems"
            :key="item"
            class="ticker-item"
          >
            {{ item }}
          </span>

          <span
            v-for="item in tickerItems"
            :key="`${item}-copy`"
            class="ticker-item"
          >
            {{ item }}
          </span>
        </div>
      </div>
    </div>
  </section>
</template>