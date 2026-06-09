<script setup>
import { ref } from 'vue'
import logo from '../assets/images/gvp_logo.png'

const isOpen = ref(false)

const closeMenu = () => {
  isOpen.value = false
}
</script>

<template>
  <header class="bg-white shadow-sm sticky top-0 z-50">
    <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
      <a href="#home" class="flex items-center gap-3" @click="closeMenu">
        <img :src="logo" alt="GVP Consult logo" class="h-14 w-auto" />
      </a>

      <nav class="hidden lg:flex gap-8 text-sm uppercase tracking-wide">
        <a href="#home">Početna</a>
        <a href="#about">O nama</a>
        <a href="#services">Usluge</a>
        <a href="#blog">Blog</a>
        <a href="#events">Događaji</a>
        <a href="#news">Vesti</a>
        <a href="#faq">FAQ</a>
        <a href="#contact">Kontakt</a>
      </nav>

      <div class="hidden lg:flex items-center gap-4">
        <a
          href="https://www.linkedin.com/in/gordana-vrastanovic-pavicevic-48698171/"
          target="_blank"
          rel="noopener noreferrer"
          class="hover:opacity-80"
          aria-label="LinkedIn profil"
        >
          <span class="inline-flex items-center justify-center w-8 h-8 rounded bg-[#0A66C2] text-white font-bold">
            in
          </span>
        </a>

        <a
          href="#contact"
          class="bg-orange-500 hover:bg-orange-600 text-white px-5 py-3 rounded"
        >
          Zakažite konsultacije
        </a>
      </div>

      <button
        type="button"
        class="lg:hidden inline-flex items-center justify-center w-10 h-10 rounded border border-gray-300 text-gray-700"
        @click="isOpen = !isOpen"
        aria-label="Otvori navigaciju"
      >
        <span v-if="!isOpen" class="text-2xl leading-none">☰</span>
        <span v-else class="text-2xl leading-none">×</span>
      </button>
    </div>

    <div
      v-if="isOpen"
      class="lg:hidden bg-white border-t border-gray-200 shadow-md"
    >
      <nav class="px-6 py-5 flex flex-col gap-4 text-sm uppercase tracking-wide">
        <a href="#home" @click="closeMenu">Početna</a>
        <a href="#about" @click="closeMenu">O nama</a>
        <a href="#services" @click="closeMenu">Usluge</a>
        <a href="#blog" @click="closeMenu">Blog</a>
        <a href="#events" @click="closeMenu">Događaji</a>
        <a href="#news" @click="closeMenu">Vesti</a>
        <a href="#faq" @click="closeMenu">FAQ</a>
        <a href="#contact" @click="closeMenu">Kontakt</a>

        <div class="pt-4 border-t border-gray-200 flex items-center gap-4">
          <a
            href="https://www.linkedin.com/in/gordana-vrastanovic-pavicevic-48698171/"
            target="_blank"
            rel="noopener noreferrer"
            class="hover:opacity-80"
            aria-label="LinkedIn profil"
          >
            <span class="inline-flex items-center justify-center w-8 h-8 rounded bg-[#0A66C2] text-white font-bold">
              in
            </span>
          </a>

          <a
            href="#contact"
            class="bg-orange-500 hover:bg-orange-600 text-white px-5 py-3 rounded"
            @click="closeMenu"
          >
            Zakažite konsultacije
          </a>
        </div>
      </nav>
    </div>
  </header>
</template>