<script setup>
import { CalendarDays, GraduationCap, Users } from '@lucide/vue'

import bezbednost from '../assets/images/bezbednost.jpg'
import kozmetika from '../assets/images/cosmetics.jpg'
import seminar from '../assets/images/seminar.jpg'

const events = [
  {
  icon: GraduationCap,
  image: bezbednost,
  contain: true,
  title: 'Bezbednost predmeta opšte upotrebe',
  text: 'Edukativni sadržaji o pravilnom razumevanju hemije, bezbednosti proizvoda i odgovornom informisanju potrošača.'
},
  {
    icon: CalendarDays,
    image: kozmetika,
    title: 'Kozmetika, suplementi i online prodaja',
    text: 'Stručna upozorenja i edukacije o reklamiranju proizvoda, dokumentaciji i rizicima kupovine putem društvenih mreža.'
  },
  {
    icon: Users,
    image: seminar,
    title: 'Seminari i stručna savetovanja',
    text: 'Učešće na stručnim seminarima iz oblasti ambalaže, kozmetike, deterdženata, obeležavanja i regulatorne usklađenosti.'
  }
]
</script>

<template>
  <section id="events" class="pt-12 pb-16 bg-white">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center mb-12">
        <span class="uppercase text-orange-500 tracking-widest text-sm">
          Događaji i edukacije
        </span>

        <h2 class="text-4xl font-serif font-bold mt-4 text-[#222222]">
          Seminari, konferencije i stručna savetovanja
        </h2>

        <div class="section-divider"></div>

        <p class="text-gray-600 max-w-3xl mx-auto mt-5 leading-relaxed">
          GVP Consult prati aktuelne regulatorne teme i učestvuje u stručnim
          edukacijama, seminarima i savetovanjima namenjenim proizvođačima,
          distributerima, laboratorijama i potrošačima.
        </p>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        <article
          v-for="event in events"
          :key="event.title"
          class="bg-[#f8f5f1] rounded-xl overflow-hidden shadow card-hover"
        >
          <div class="relative">
            <img
              :src="event.image"
              :alt="event.title"
              :class="[
                event.contain
                  ? 'h-80 w-full object-contain bg-[#eef4df] p-3'
                  : 'h-56 w-full object-cover'
              ]"
            />

            <div
              class="absolute -bottom-7 left-7 w-14 h-14 rounded-full bg-white shadow-lg flex items-center justify-center"
            >
              <component
                :is="event.icon"
                class="w-7 h-7 text-orange-500"
              />
            </div>
          </div>

          <div class="p-7 pt-10">
            <h3 class="font-semibold text-xl mb-3 text-[#222222]">
              {{ event.title }}
            </h3>

            <p class="text-gray-600 leading-relaxed">
              {{ event.text }}
            </p>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>