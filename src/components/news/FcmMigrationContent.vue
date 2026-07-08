<script setup>
import coverImage from '../../assets/images/news/2026-07-06-fcm-migration-content.jpg'
</script>

<template>
  <article class="bg-white rounded-xl shadow-lg overflow-hidden">

    <img
      :src="coverImage"
      alt="FCM: Migracija supstance nije isto što i sadržaj supstance"
      class="w-full h-64 object-cover"
    />

    <div class="p-8">

      <div class="flex flex-wrap items-center gap-3 text-sm text-gray-500 mb-4">
        <span>06.07.2026.</span>
        <span>•</span>
        <span class="font-semibold text-orange-600">
          FCM / MATERIJALI U KONTAKTU SA HRANOM
        </span>
      </div>

      <h3 class="text-3xl font-serif font-bold mb-6">
        FCM: Migracija supstance nije isto što i sadržaj supstance
      </h3>

      <p class="text-gray-700 leading-8 mb-6">
        U praksi se često susreću izveštaji o ispitivanju i Declaration of
        Conformity (DoC) dokumentacija u kojima se mešaju pojmovi sadržaja i
        migracije određene supstance. Međutim, to nisu ista ispitivanja, niti
        daju iste informacije.
      </p>

      <div class="grid md:grid-cols-2 gap-6 mb-8">

        <div class="bg-green-50 border-l-4 border-green-600 p-5 rounded">
          <h4 class="text-xl font-semibold mb-3">
            Sadržaj supstance
          </h4>

          <p class="text-gray-700 leading-7">
            Sadržaj pokazuje koliko se određene supstance ukupno nalazi u
            materijalu ili predmetu. Određivanje se najčešće vrši razaranjem
            ili rastvaranjem osnovnog materijala, a zatim izolovanjem supstance
            koja se određuje.
          </p>
        </div>

        <div class="bg-blue-50 border-l-4 border-blue-600 p-5 rounded">
          <h4 class="text-xl font-semibold mb-3">
            Migracija supstance
          </h4>

          <p class="text-gray-700 leading-7">
            Migracija pokazuje mogućnost da supstanca, pod definisanim uslovima
            ispitivanja, pređe iz materijala u simulant hrane ili u samu hranu.
            Ispitivanje se vrši bez razaranja osnovnog materijala.
          </p>
        </div>

      </div>

      <h4 class="text-xl font-semibold mb-4">
        Šta je važno za procenu usaglašenosti?
      </h4>

      <ul class="list-disc ml-6 space-y-3 text-gray-700 mb-8 leading-7">
        <li>da li je ispitivan sadržaj ili migracija supstance,</li>
        <li>koja je analitička metoda primenjena,</li>
        <li>da li metoda odgovara zahtevima važeće regulative,</li>
        <li>da li su korišćeni odgovarajući simulanti, vreme i temperatura ispitivanja,</li>
        <li>kako pravilno interpretirati rezultate i preneti ih u Declaration of Conformity (DoC).</li>
      </ul>

      <h4 class="text-xl font-semibold mb-4">
        Stručni komentar GVP Consult
      </h4>

      <div class="bg-orange-50 border-l-4 border-orange-500 p-6 rounded">

        <p class="text-gray-700 leading-8">
          Sam broj u laboratorijskom izveštaju nije dovoljan. Potrebno je
          razumeti kako je rezultat dobijen, kojom metodom, pod kojim uslovima
          i da li je relevantan za dokazivanje usaglašenosti proizvoda.
        </p>

        <p class="text-gray-700 leading-8 mt-4">
          Zahtevi nisu isti u svim propisima. Neke regulative postavljaju
          ograničenja za ukupan sadržaj određene supstance, dok druge propisuju
          granične vrednosti migracije. Pogrešno tumačenje ovih zahteva može
          dovesti do pogrešne procene usaglašenosti proizvoda.
        </p>

      </div>

      <p class="text-gray-700 leading-8 mt-8">
        Razumevanje razlike između migracije i sadržaja jedan je od osnovnih
        preduslova za pravilno tumačenje laboratorijskih izveštaja, pripremu
        kvalitetne DoC dokumentacije i donošenje pouzdanih odluka o
        usaglašenosti proizvoda.
      </p>

    </div>

  </article>
</template>