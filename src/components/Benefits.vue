<script setup>
import {
  Award,
  ShieldCheck,
  Lightbulb,
  Users,
  BriefcaseBusiness
} from '@lucide/vue'

const benefits = [
  {
    icon: Award,
    title: 'Stručno iskustvo'
  },
  {
    icon: ShieldCheck,
    title: 'Regulatorna usklađenost'
  },
  {
    icon: Lightbulb,
    title: 'Praktična rešenja'
  },
  {
    icon: Users,
    title: 'Individualni pristup'
  },
  {
    icon: BriefcaseBusiness,
    title: 'Podrška poslovanju'
  }
]
</script>

<template>
  <section class="bg-[#222222] text-white py-12">

    <div class="max-w-7xl mx-auto px-6">

      <div
        class="grid sm:grid-cols-2 lg:grid-cols-5 gap-8 text-center"
      >

        <div
          v-for="item in benefits"
          :key="item.title"
          class="group"
        >

          <component
            :is="item.icon"
            class="w-12 h-12 mx-auto mb-4 text-orange-400 group-hover:scale-110 transition"
          />

          <h3 class="font-semibold">
            {{ item.title }}
          </h3>

        </div>

      </div>

    </div>

  </section>
</template>