<script setup>
import gocaImage from '../assets/images/goca1.jpg'
</script>

<template>
  <section id="about" class="bg-white py-20">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-12 items-center">
      <img
        :src="gocaImage"
        alt="Gordana Vraštanović Pavićević"
        class="rounded-lg shadow-xl w-full h-[540px] object-cover object-top"
      />

      <div>
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          O nama
        </span>

        <h2 class="text-4xl font-serif font-bold mt-4 mb-4 text-[#222222]">
          Gordana Vraštanović Pavićević
        </h2>

        <p class="text-lg font-semibold text-orange-600 mb-6">
          Specijalista sanitarne hemije · Stručni konsultant za bezbednost proizvoda
        </p>

        <p class="text-gray-700 mb-4 leading-relaxed">
          GVP Consult pruža stručnu podršku sektorima za kontrolu kvaliteta,
          uvoz, izvoz, proveru dokumentacije i izradu deklaracija o usaglašenosti.
        </p>

        <p class="text-gray-700 mb-6 leading-relaxed">
          Poseban fokus je na predmetima opšte upotrebe, ambalaži za hranu,
          kozmetičkim proizvodima, igračkama, laboratorijskim analizama i proizvodima
          koji dolaze u kontakt sa kožom i sluzokožom.
        </p>

        <div class="flex flex-wrap gap-4">
        <a
            href="/biografija.html"
            target="_blank"
            rel="noopener noreferrer"
            class="inline-block bg-orange-500 text-white px-6 py-3 rounded hover:bg-orange-600"
            >
            Biografija
        </a>

          <a
            href="#contact"
            class="inline-block border border-orange-500 text-orange-600 px-6 py-3 rounded hover:bg-orange-500 hover:text-white"
          >
            Kontaktirajte nas
          </a>
        </div>
      </div>
    </div>
  </section>
</template>