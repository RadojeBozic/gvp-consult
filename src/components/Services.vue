<script setup>
import {
  PackageCheck,
  Sparkles,
  ToyBrick,
  ScanFace,
  FlaskConical,
  FileCheck2
} from '@lucide/vue'

import posudjeZaHranu from '../assets/images/posudje_za_hranu.jpg'
import kozmetickiProizvodi from '../assets/images/kozmeticki_proizvodi.jpg'
import proizvodiZaDecu from '../assets/images/proizvodi_za_decu.jpg'
import nakitBizuterija from '../assets/images/nakit_bizuterija.jpg'
import laboratorije from '../assets/images/laboratorije.jpg'
import docDokumentacija from '../assets/images/doc_dokumentacija.jpg'

const services = [
  {
    icon: PackageCheck,
    image: posudjeZaHranu,
    title: 'Ambalaža i posuđe za hranu',
    text: 'Provera dokumentacije, DoC deklaracije i usklađenosti materijala koji dolaze u kontakt sa hranom.'
  },
  {
    icon: Sparkles,
    image: kozmetickiProizvodi,
    title: 'Kozmetički proizvodi',
    text: 'Podrška u vezi sa PIF dokumentacijom, deklarisanjem, bezbednošću i regulatornim zahtevima.'
  },
  {
    icon: ToyBrick,
    image: proizvodiZaDecu,
    title: 'Igračke i proizvodi za decu',
    text: 'Savetovanje u vezi sa bezbednosnim zahtevima, dokumentacijom i rizicima kod proizvoda namenjenih deci.'
  },
  {
    icon: ScanFace,
    image: nakitBizuterija,
    title: 'Kontakt sa kožom i sluzokožom',
    text: 'Nakit, bižuterija, pelene, ulošci, brijači, boje za tetovažu, pirsing i srodni proizvodi.'
  },
  {
    icon: FlaskConical,
    image: laboratorije,
    title: 'Laboratorije',
    text: 'Stručna podrška laboratorijama u vezi sa ispitivanjima, metodama, dokumentacijom i komunikacijom sa klijentima.'
  },
  {
    icon: FileCheck2,
    image: docDokumentacija,
    title: 'DoC dokumentacija',
    text: 'Izrada i provera deklaracija o usaglašenosti i prateće dokumentacije za proizvode i ambalažu.'
  }
]
</script>

<template>
  <section id="services" class="pt-4 pb-16 bg-[#f8f5f1]">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center mb-12">
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          Usluge
        </span>

        <h2 class="text-4xl font-serif font-bold mt-4 text-[#222222]">
          Oblasti stručne podrške
        </h2>

        <div class="section-divider"></div>

        <p class="text-gray-600 max-w-3xl mx-auto mt-5 leading-relaxed">
          Konsultantska podrška obuhvata proveru dokumentacije, regulatornu
          usklađenost, komunikaciju sa laboratorijama i praktične smernice za
          bezbedno stavljanje proizvoda na tržište.
        </p>
      </div>

      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <article
          v-for="service in services"
          :key="service.title"
          class="bg-white rounded-xl overflow-hidden shadow card-hover"
        >
          <div class="relative">
            <img
              :src="service.image"
              :alt="service.title"
              class="h-52 w-full object-cover"
            />

            <div
              class="absolute -bottom-7 left-7 w-14 h-14 rounded-full bg-white shadow-lg flex items-center justify-center"
            >
              <component
                :is="service.icon"
                class="w-7 h-7 text-orange-500"
              />
            </div>
          </div>

          <div class="p-7 pt-10">
            <h3 class="text-xl font-semibold mb-3 text-[#222222]">
              {{ service.title }}
            </h3>

            <p class="text-gray-600 leading-relaxed">
              {{ service.text }}
            </p>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>