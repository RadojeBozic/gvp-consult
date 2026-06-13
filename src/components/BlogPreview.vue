<script setup>
import bezbednaAmbalaza from '../assets/images/bezbedna_ambalaza.jpg'
import izmeneKozmetika from '../assets/images/izmene_kozmetika.jpg'
import kozmetika from '../assets/images/kozmetika.jpg'
import nebezbednaAmbalaza from '../assets/images/nebezbedna_ambalaza.jpg'
import pfas from '../assets/images/pfas.jpg'
import ppwr from '../assets/images/ppwr.jpg'

const posts = [
    {
    image: bezbednaAmbalaza,
    category: 'DoC · Ambalaža',
    title: 'Deklaracija o usaglašenosti za ambalažu za pakovanje hrane',
    excerpt:
      'Zašto DoC nije samo formalnost, već ključni dokaz bezbednosti, sledljivosti i regulatorne usklađenosti.',
    link: '/blog/deklaracija-o-usaglasenosti-doc.html'
  },
  {
  image: izmeneKozmetika,
  category: 'Kozmetika · EU regulativa',
  title: 'Izmene u EU regulativi 1223/2009 za kozmetičke proizvode',
  excerpt:
    'Pregled važnih izmena u aneksima i njihov značaj za proizvođače, uvoznike i distributere kozmetike.',
    link: '/blog/izmene-eu-regulative-1223-2009.html'
},
 {
  image: kozmetika,
  category: 'E-commerce · Potrošači',
  title: 'Kupujete kozmetiku, suplemente ili „kreme koje leče“?',
  excerpt:
    'Instagram i online prodaja nisu dokaz kvaliteta i bezbednosti proizvoda. Pre kupovine proverite dokumentaciju.',
    link: '/blog/instagram-kozmetika-i-bezbednost-proizvoda.html'
},
  {
    image: nebezbednaAmbalaza,
    category: 'Ambalaža · Rizici',
    title: 'Da li vaša ambalaža ima potvrdu da je bezbedna za hranu?',
    excerpt:
      'Bez odgovarajuće dokumentacije mogu nastati problemi kod HACCP, IFS provera, izvoza i inspekcijskih kontrola.',
    link: '/blog/ambalaza-bezbedna-za-hranu.html'
  },
  {
  image: pfas,
  category: 'PFAS · Laboratorije',
  title: 'PFAS, PPWR i izazovi laboratorijskih ispitivanja',
  excerpt:
    'Zašto nejasna metodologija može proizvođačima i laboratorijama stvoriti dodatne troškove i regulatornu nesigurnost.',
  link: '/blog/pfas-ppwr-i-laboratorijska-ispitivanja.html'
},
  {
  image: ppwr,
  category: 'PPWR · Regulativa',
  title: 'PPWR član 5 tačka 5 — kamen spoticanja za ambalažu',
  excerpt:
    'Novi zahtevi za ambalažu za hranu otvaraju ozbiljna pitanja o metodologiji, analizama i dokazivanju usklađenosti.',
  link: '/blog/ppwr-clan-5-tacka-5.html'
},
]
</script>

<template>
  <section id="blog" class="pt-10 pb-16 bg-white">
    <div class="max-w-7xl mx-auto px-6">

      <div class="text-center mb-14">
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          Blog
        </span>

        <h2 class="text-4xl font-serif font-bold mt-4 text-[#222222]">
          Stručni tekstovi i edukacije
        </h2>

        <div class="section-divider"></div>

        <p class="text-gray-600 max-w-3xl mx-auto mt-5 leading-relaxed">
          Aktuelne teme iz oblasti bezbednosti proizvoda, regulatorne
          usklađenosti, ambalaže za hranu, kozmetičkih proizvoda,
          laboratorijskih ispitivanja i zaštite potrošača.
        </p>
      </div>

      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <article
          v-for="post in posts"
          :key="post.title"
          class="bg-[#f8f5f1] rounded-xl overflow-hidden shadow card-hover"
        >
          <div class="bg-white">
            <img
              :src="post.image"
              :alt="post.title"
              class="h-64 w-full object-cover"
            />
          </div>

          <div class="p-6">
            <span class="inline-block text-xs uppercase tracking-widest text-orange-500 font-semibold mb-3">
              {{ post.category }}
            </span>

            <h3 class="text-xl font-semibold text-[#222222] mb-3 leading-snug">
              {{ post.title }}
            </h3>

            <p class="text-gray-600 leading-relaxed mb-5">
              {{ post.excerpt }}
            </p>

            <a
              :href="post.link"
              class="font-semibold text-orange-600 hover:text-orange-700"
            >
              Pročitajte više →
            </a>
          </div>
        </article>
      </div>

      <div class="text-center mt-12">
        <a
          href="#"
          class="inline-block bg-orange-500 hover:bg-orange-600 text-white px-8 py-3 rounded-lg transition"
        >
          Pogledajte sve tekstove
        </a>
      </div>

    </div>
  </section>
</template>