<script setup>
import {
  PackageCheck,
  Sparkles,
  ToyBrick,
  ScanFace,
  FlaskConical,
  FileCheck2
} from '@lucide/vue'

const services = [
  {
    icon: PackageCheck,
    title: 'Ambalaža i posuđe za hranu',
    text: 'Provera dokumentacije, DoC deklaracije i usklađenosti materijala koji dolaze u kontakt sa hranom.'
  },
  {
    icon: Sparkles,
    title: 'Kozmetički proizvodi',
    text: 'Podrška u vezi sa PIF dokumentacijom, deklarisanjem, bezbednošću i regulatornim zahtevima.'
  },
  {
    icon: ToyBrick,
    title: 'Igračke i proizvodi za decu',
    text: 'Savetovanje u vezi sa bezbednosnim zahtevima, dokumentacijom i rizicima kod proizvoda namenjenih deci.'
  },
  {
    icon: ScanFace,
    title: 'Kontakt sa kožom i sluzokožom',
    text: 'Nakit, bižuterija, pelene, ulošci, brijači, boje za tetovažu, pirsing i srodni proizvodi.'
  },
  {
    icon: FlaskConical,
    title: 'Laboratorije',
    text: 'Stručna podrška laboratorijama u vezi sa ispitivanjima, metodama, dokumentacijom i komunikacijom sa klijentima.'
  },
  {
    icon: FileCheck2,
    title: 'DoC dokumentacija',
    text: 'Izrada i provera deklaracija o usaglašenosti i prateće dokumentacije za proizvode i ambalažu.'
  }
]
</script>

<template>
  <section id="services" class="py-20 bg-[#f8f5f1]">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center mb-14">
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          Usluge
        </span>

        <h2 class="text-4xl font-serif font-bold mt-4 text-[#222222]">
          Oblasti stručne podrške
        </h2>

        <p class="text-gray-600 max-w-3xl mx-auto mt-5 leading-relaxed">
          Konsultantska podrška obuhvata proveru dokumentacije, regulatornu
          usklađenost, komunikaciju sa laboratorijama i praktične smernice za
          bezbedno stavljanje proizvoda na tržište.
        </p>
      </div>

      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div
          v-for="service in services"
          :key="service.title"
          class="bg-white p-7 rounded-lg shadow hover:shadow-lg transition"
        >
          <component :is="service.icon" class="w-9 h-9 text-orange-500 mb-5" />

          <h3 class="text-xl font-semibold mb-3 text-[#222222]">
            {{ service.title }}
          </h3>

          <p class="text-gray-600 leading-relaxed">
            {{ service.text }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>