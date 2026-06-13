<script setup>
import gocaImage from '../assets/images/goca3.jpg'
</script>

<template>
  <section id="biografija" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-12 items-start">
      <div>
        <img
          :src="gocaImage"
          alt="Gordana Vraštanović Pavićević"
          class="rounded-lg shadow-xl w-full h-[560px] object-cover object-top"
        />
      </div>

      <div>
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          Biografija
        </span>

        <h2 class="text-4xl font-serif font-bold mt-4 mb-5 text-[#222222]">
          Gordana Vraštanović Pavićević
        </h2>

        <p class="text-lg font-semibold text-orange-600 mb-6">
          Specijalista sanitarne hemije · Konsultant za bezbednost proizvoda i regulatornu usklađenost
        </p>

        <p class="text-gray-700 leading-relaxed mb-4">
          Gordana Vraštanović Pavićević je stručni saradnik i konsultant u oblasti
          laboratorijskih ispitivanja, kontrole kvaliteta, uvoza, izvoza,
          provere dokumentacije i izrade deklaracija o usaglašenosti.
        </p>

        <p class="text-gray-700 leading-relaxed mb-4">
          Kroz GVP Consult pruža podršku proizvođačima, uvoznicima, distributerima,
          laboratorijama i sektorima za kontrolu kvaliteta u vezi sa bezbednošću
          predmeta opšte upotrebe, ambalaže za hranu, kozmetičkih proizvoda,
          igračaka i proizvoda koji dolaze u kontakt sa kožom i sluzokožom.
        </p>

        <p class="text-gray-700 leading-relaxed mb-8">
          Posebno se bavi regulatornom usklađenošću, DoC dokumentacijom,
          procenom rizika, komunikacijom sa laboratorijama i tumačenjem zahteva
          domaćih i evropskih propisa.
        </p>

        <div class="grid sm:grid-cols-2 gap-4">
          <div class="bg-[#f8f5f1] p-5 rounded-lg">
            <h3 class="font-semibold mb-2">Stručne oblasti</h3>
            <p class="text-gray-600 text-sm">
              Ambalaža za hranu, kozmetika, igračke, proizvodi za kontakt sa kožom.
            </p>
          </div>

          <div class="bg-[#f8f5f1] p-5 rounded-lg">
            <h3 class="font-semibold mb-2">Dokumentacija</h3>
            <p class="text-gray-600 text-sm">
              DoC, PIF, provera usklađenosti i priprema prateće dokumentacije.
            </p>
          </div>

          <div class="bg-[#f8f5f1] p-5 rounded-lg">
            <h3 class="font-semibold mb-2">Laboratorije</h3>
            <p class="text-gray-600 text-sm">
              Podrška u vezi sa analizama, metodama ispitivanja i tumačenjem rezultata.
            </p>
          </div>

          <div class="bg-[#f8f5f1] p-5 rounded-lg">
            <h3 class="font-semibold mb-2">Edukacije</h3>
            <p class="text-gray-600 text-sm">
              Učešće na stručnim skupovima, seminarima, konferencijama i savetovanjima.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>