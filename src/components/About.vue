<script setup>
import {
  CheckCircle2,
  FileCheck2,
  FlaskConical,
  GraduationCap,
  Scale,
  ShieldCheck
} from '@lucide/vue'

import gocaImage from '../assets/images/goca4.png'

const highlights = [
  {
    icon: ShieldCheck,
    title: 'Višedecenijsko iskustvo',
    text: 'Iskustvo u oblasti bezbednosti predmeta opšte upotrebe, primeni i tumačenju propisa Republike Srbije i EU.'
  },
  {
    icon: FlaskConical,
    title: 'Laboratorijska praksa',
    text: 'Iskustvo kao analitičar i rukovodilac, u razvoju metoda, tumačenju rezultata ispitivanja, davanju stručnih mišljenja i akreditaciji u skladu sa SRPS EN 17025.'
  },
  {
    icon: Scale,
    title: 'Nacionalni propisi',
    text: 'Aktivni učesnik izrade nacionalnih propisa iz oblasti predmeta opšte upotrebe.'
  },
  {
    icon: FileCheck2,
    title: 'DoC, PIF i dokumentacija',
    text: 'Iskustvo u formiranju DoC, delova za dosije sa informacijama o proizvodu (PIF) i druge regulatorne dokumentacije.'
  },
  {
    icon: GraduationCap,
    title: 'Predavanja i edukacije',
    text: 'Stručna predavanja, edukacije, seminari, obuke i savetovanja.'
  },
  {
    icon: CheckCircle2,
    title: 'Praktična rešenja',
    text: 'Praktična rešenja za proizvođače, uvoznike, distributere i laboratorije.'
  }
]
</script>

<template>
  <section id="about" class="bg-white pt-12 pb-10">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-12 items-center">
      <div class="relative max-w-md mx-auto lg:mx-0">
        <div class="absolute -right-5 -bottom-5 w-full h-full bg-orange-100 rounded-2xl"></div>

        <img
          :src="gocaImage"
          alt="Gordana Vraštanović Pavićević"
          class="relative rounded-2xl shadow-xl w-full object-cover object-center"
        />
      </div>

      <div>
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          Ko stoji iza GVP Consult?
        </span>

        <h2 class="text-4xl font-serif font-bold mt-4 mb-4 text-[#222222]">
          Gordana Vraštanović Pavićević, dipl. hem.
        </h2>

        <p class="text-lg font-semibold text-orange-600 mb-6">
          Specijalista sanitarne hemije · PR GVP CONSULT
        </p>

        <p class="text-gray-700 mb-4 leading-relaxed">
          GVP Consult pruža stručnu podršku proizvođačima, uvoznicima,
          distributerima i laboratorijama u oblasti bezbednosti predmeta opšte
          upotrebe, regulatorne usklađenosti, dokumentacije i kontrole kvaliteta.
        </p>

        <p class="text-gray-700 mb-6 leading-relaxed">
          Fokus konsultantskog rada je na praktičnoj primeni propisa,
          smanjenju poslovnih rizika, pravilnoj pripremi dokumentacije i
          sigurnijem plasmanu proizvoda na tržište.
        </p>

        <div class="grid sm:grid-cols-2 gap-4 mb-8">
          <div
            v-for="item in highlights"
            :key="item.title"
            class="bg-[#f8f5f1] rounded-xl p-4 border border-orange-100"
          >
            <component
              :is="item.icon"
              class="w-6 h-6 text-orange-500 mb-3"
            />

            <h3 class="font-semibold text-[#222222] mb-2">
              {{ item.title }}
            </h3>

            <p class="text-sm text-gray-700 leading-relaxed">
              {{ item.text }}
            </p>
          </div>
        </div>

        <div class="flex flex-wrap gap-4">
          <a
            href="/biografija.html"
            target="_blank"
            rel="noopener noreferrer"
            class="inline-block bg-orange-500 text-white px-6 py-3 rounded hover:bg-orange-600 transition"
          >
            Detaljna biografija
          </a>

          <a
            href="#contact"
            class="inline-block border border-orange-500 text-orange-600 px-6 py-3 rounded hover:bg-orange-500 hover:text-white transition"
          >
            Zakažite konsultacije
          </a>
        </div>
      </div>
    </div>
  </section>
</template>