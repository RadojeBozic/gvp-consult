<script setup>
import heroImage from '../assets/images/hero1.jpg'
import { ShieldCheck, FileCheck2 } from '@lucide/vue'
</script>

<template>
  <section id="home" class="bg-[#f8f5f1]">
    <div class="max-w-7xl mx-auto px-6 py-24 grid lg:grid-cols-2 gap-14 items-center">
      <div>
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          GVP Consult
        </span>

        <h1
          class="text-4xl md:text-5xl xl:text-6xl
                font-serif font-bold
                leading-tight
                mb-6"
        >
          Bezbednost proizvoda.
          <br>
          Sigurnost poslovanja.
        </h1>
        <p class="text-gray-700 text-lg leading-relaxed mb-8">
          Stručna podrška proizvođačima, uvoznicima, distributerima i laboratorijama
          u oblasti predmeta opšte upotrebe, ambalaže za hranu, kozmetike, igračaka
          i proizvoda koji dolaze u kontakt sa kožom i sluzokožom.
        </p>

        <div class="grid sm:grid-cols-2 gap-4 mb-9">
          <div class="flex items-start gap-3">
            <ShieldCheck class="w-6 h-6 text-orange-500 mt-1" />
            <p class="text-gray-700">Procena rizika i usklađenosti proizvoda</p>
          </div>

          <div class="flex items-start gap-3">
            <FileCheck2 class="w-6 h-6 text-orange-500 mt-1" />
            <p class="text-gray-700">DoC, PIF i prateća dokumentacija</p>
          </div>
        </div>

        <div class="flex flex-wrap gap-4">
          <a href="#contact" class="bg-orange-500 text-white px-7 py-3 rounded hover:bg-orange-600">
            Zakažite konsultacije
          </a>

          <a href="#services" class="border border-gray-700 px-7 py-3 rounded hover:bg-gray-900 hover:text-white">
            Pogledajte usluge
          </a>
        </div>
      </div>

      <div>
        <img
          :src="heroImage"
          alt="GVP Consult stručno predavanje"
          class="rounded-lg shadow-2xl w-full h-[420px]"
        />
      </div>
    </div>
  </section>
</template>