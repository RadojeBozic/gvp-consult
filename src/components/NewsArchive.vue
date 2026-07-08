<script setup>
import PetRecycledContent from './news/PetRecycledContent.vue'
import FcmMigrationContent from './news/FcmMigrationContent.vue'
</script>

<template>
<section id="news" class="py-20 bg-[#f8f5f1]">

  <div class="max-w-7xl mx-auto px-6">

    <div class="text-center mb-12">
      <span class="uppercase text-orange-500 tracking-widest text-sm">
        Aktuelnosti
      </span>

      <h2 class="text-4xl font-serif font-bold mt-4">
        Stručne novosti i regulatorne informacije
      </h2>
    </div>

    <div class="section-divider"></div>

    <div class="grid lg:grid-cols-2 gap-10">

      <PetRecycledContent />
      <FcmMigrationContent />

    </div>

  </div>

</section>
</template>