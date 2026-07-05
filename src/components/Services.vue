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
    lead: 'Materijali i predmeti za kontakt sa hranom, Food Contact Materials (FCM).',
    items: [
      'Menadžment testiranjem',
      'Provera izveštaja o ispitivanju i usklađenosti sa propisima Republike Srbije i/ili EU',
      'Mapiranje tehničke dokumentacije',
      'Formiranje Deklaracije o usaglašenosti (DoC)',
      'Priprema nacrta deklaracije i uputstva za upotrebu, u skladu sa propisima',
      'Pomoć pri formiranju dokumenta o Dobroj proizvođačkoj praksi (GMP zahtevi)',
      'Druge savetodavne usluge u cilju poslovanja usklađenog sa relevantnim propisima'
    ]
  },
  {
    icon: Sparkles,
    image: kozmetickiProizvodi,
    title: 'Kozmetički proizvodi',
    lead: 'Podrška u vezi sa bezbednošću, dokumentacijom, PIF dosijeom i regulatornim zahtevima.',
    items: [
      'Menadžment testiranjem',
      'Provera izveštaja o ispitivanju i usklađenosti sa propisima Republike Srbije i/ili EU',
      'Mapiranje tehničke dokumentacije',
      'Plan aktivnosti u cilju izrade Dosijea sa informacijama o proizvodu (PIF)',
      'Priprema nacrta deklaracije u skladu sa propisima',
      'Pomoć pri formiranju dokumenta o Dobroj proizvođačkoj praksi (GMP zahtevi)',
      'Pomoć pri kategorizaciji graničnih proizvoda',
      'Druge savetodavne usluge u cilju poslovanja usklađenog sa relevantnim propisima'
    ]
  },
  {
    icon: ToyBrick,
    image: proizvodiZaDecu,
    title: 'Igračke i proizvodi za decu',
    lead: 'Savetovanje u vezi sa dokumentacijom, testiranjem i zahtevima za proizvode namenjene deci.',
    items: [
      'Menadžment testiranjem',
      'Provera izveštaja o ispitivanju i usklađenosti sa propisima Republike Srbije i/ili EU',
      'Mapiranje tehničke dokumentacije',
      'Plan aktivnosti u cilju izrade Deklaracije o usaglašenosti',
      'Priprema nacrta deklaracije u skladu sa propisima',
      'Pomoć pri formiranju dokumenta o Dobroj proizvođačkoj praksi (GMP zahtevi)',
      'Pomoć pri kategorizaciji graničnih proizvoda',
      'Druge savetodavne usluge u cilju poslovanja usklađenog sa relevantnim propisima'
    ]
  },
  {
    icon: ScanFace,
    image: nakitBizuterija,
    title: 'Kontakt sa kožom i sluzokožom',
    lead: 'Predmeti namenjeni za kontakt sa kožom i sluzokožom, uključujući nakit i boje za tetovažu.',
    items: [
      'Menadžment testiranjem',
      'Provera izveštaja o ispitivanju i usklađenosti sa propisima Republike Srbije i/ili EU',
      'Mapiranje tehničke dokumentacije',
      'Plan aktivnosti u cilju izrade Deklaracije o usklađenosti',
      'Priprema nacrta deklaracije u skladu sa propisima',
      'Pomoć pri formiranju dokumenta o Dobroj proizvođačkoj praksi (GMP zahtevi)',
      'Pomoć pri kategorizaciji graničnih proizvoda',
      'Druge savetodavne usluge u cilju poslovanja usklađenog sa relevantnim propisima'
    ]
  },
  {
    icon: FlaskConical,
    image: laboratorije,
    title: 'Laboratorije',
    lead: 'Podrška laboratorijama za ispitivanje bezbednosti, usaglašenosti i zdravstvene ispravnosti.',
    items: [
      'Stručna podrška planiranju razvoja i proširenja obima akreditacije i obima ispitivanja',
      'Validacija metoda, analiza rezultata ispitivanja i stručna podrška u tumačenju propisa',
      'Stručna pomoć u planiranju razvoja laboratorija',
      'Kontinualno praćenje propisa iz oblasti ekspertiza',
      'Stručna pomoć za izjave o usaglašenosti proizvoda i stručna mišljenja na osnovu rezultata ispitivanja'
    ]
  },
  {
    icon: FileCheck2,
    image: docDokumentacija,
    title: 'Kontrola kvaliteta i regulatorna usklađenost',
    lead: 'Tumačenje domaćih i EU propisa, procena rizika i stručna savetovanja.',
    items: [
      'Tumačenje rezultata ispitivanja i usklađenosti sa domaćim i EU propisima',
      'Menadžment testiranjem',
      'Zastupanje kod nadležnih inspekcijskih organa po potrebi',
      'Komunikacija sa Ministarstvom zdravlja po potrebi',
      'Obuka o usklađenosti sa propisima o bezbednosti proizvoda prema potrebama klijenta'
    ]
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

      <div class="grid lg:grid-cols-2 gap-8">
        <article
          v-for="service in services"
          :key="service.title"
          class="bg-white rounded-xl overflow-hidden shadow card-hover"
        >
          <div class="relative">
            <img
              :src="service.image"
              :alt="service.title"
              class="h-56 w-full object-cover"
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

            <p class="text-gray-600 leading-relaxed mb-5">
              {{ service.lead }}
            </p>

            <ul class="space-y-2">
              <li
                v-for="item in service.items"
                :key="item"
                class="flex gap-3 text-gray-700 leading-relaxed"
              >
                <span class="text-orange-500 mt-1 shrink-0">✓</span>
                <span>{{ item }}</span>
              </li>
            </ul>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>