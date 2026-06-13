<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Services from './components/Services.vue'
import Benefits from './components/Benefits.vue'
import Events from './components/Events.vue'
import NewsArchive from './components/NewsArchive.vue'
import FAQ from './components/FAQ.vue'
import UsefulLinks from './components/UsefulLinks.vue'
import Testimonials from './components/Testimonials.vue'
import BlogPreview from './components/BlogPreview.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="min-h-screen bg-[#f8f5f1] text-[#2f2f2f]">
    <Header />
    <Hero />
    <Services />
    <Benefits />
    <About />
    <BlogPreview />
    <NewsArchive />
    <FAQ />
    <Events />
    <UsefulLinks />
    <Testimonials />
    <Contact />
    <Footer />
  </div>
</template>