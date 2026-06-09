<script setup>
import logo from '../assets/images/gvp_logo.png'
import { Mail, Phone } from '@lucide/vue'
</script>

<template>
  <footer class="bg-[#222222] text-white py-12">

        <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-3 gap-10">

            <div>

            <img
                :src="logo"
                alt="GVP Consult"
                class="h-20 bg-white p-2 rounded mb-5"
            />

            <p class="text-gray-300 leading-relaxed">
                Konsultantska podrška za bezbednost proizvoda,
                regulatornu usklađenost, DoC dokumentaciju,
                kozmetičke proizvode, ambalažu za hranu i laboratorije.
            </p>

            </div>

            <div>

            <h3 class="font-semibold text-lg mb-4">
                Brza navigacija
            </h3>

            <ul class="space-y-3 text-gray-300">

                <li><a href="#home">Početna</a></li>
                <li><a href="#about">O nama</a></li>
                <li><a href="#services">Usluge</a></li>
                <li><a href="#blog">Blog</a></li>
                <li><a href="#events">Događaji</a></li>
                <li><a href="#news">Vesti</a></li>
                <li><a href="#contact">Kontakt</a></li>

            </ul>

            </div>

            <div>

            <h3 class="font-semibold text-lg mb-4">
                Kontakt
            </h3>

            <div class="space-y-4">

                <p class="flex items-center gap-3">
                <Mail class="w-5 h-5 text-orange-400" />
                gvpconsult24@gmail.com
                </p>

                <p class="flex items-center gap-3">
                <Phone class="w-5 h-5 text-orange-400" />
                +381 64 157 95 99
                </p>

                <a
                href="https://www.linkedin.com/in/gordana-vrastanovic-pavicevic-48698171/"
                target="_blank"
                rel="noopener noreferrer"
                class="flex items-center gap-3 hover:text-orange-400"
                >
                <span class="inline-flex items-center justify-center w-6 h-6 rounded bg-[#0A66C2] text-white text-sm font-bold">
                    in
                </span>
                LinkedIn profil
                </a>

            </div>

            </div>

        </div>

        <div
            class="max-w-7xl mx-auto px-6 mt-10 pt-6 border-t border-gray-700 text-center text-gray-400"
        >
            © 2026 GVP Consult · Gordana Vraštanović Pavićević · Sva prava zadržana
        </div>

        </footer>
</template>