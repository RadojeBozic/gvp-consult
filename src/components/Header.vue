<script setup>
import logo from '../assets/images/gvp_logo.png'

</script>

<template>
  <header class="bg-white shadow-sm sticky top-0 z-50">
    <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
      <a href="#home" class="flex items-center gap-3">
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

       <a
          href="https://www.linkedin.com/in/gordana-vrastanovic-pavicevic-48698171/"
          target="_blank"
          class="text-gray-700 hover:text-orange-500"
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
  </header>
</template>