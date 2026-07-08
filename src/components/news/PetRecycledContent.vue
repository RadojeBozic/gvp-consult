<script setup>
import coverImage from '../../assets/images/news/2026-07-06-pet-recycled-content.jpg'
</script>


<template>

<article class="bg-white rounded-xl shadow-lg overflow-hidden">

    <!-- Fotografija -->

     <img
    :src="coverImage"
    alt="Proračun recikliranog sadržaja u PET bocama"
    class="w-full h-64 object-cover"
  />

    <div class="p-8">

        <div class="flex flex-wrap items-center gap-3 text-sm text-gray-500 mb-4">

            <span>06.07.2026.</span>

            <span>•</span>

            <span class="font-semibold text-orange-600">
                EU REGULATIVA
            </span>

        </div>

        <h3 class="text-3xl font-serif font-bold mb-6">

            Proračun recikliranog sadržaja u PET bocama za jednokratnu upotrebu

        </h3>

        <p class="text-gray-700 leading-8 mb-6">

            Evropska komisija objavila je metodologiju za izračunavanje,
            verifikaciju i izveštavanje o sadržaju hemijski reciklirane
            plastike u jednokratnim PET bocama za piće.

            Cilj nove odluke jeste uspostavljanje jedinstvenih pravila
            za sve države članice Evropske unije, povećanje pravne sigurnosti
            i podsticanje ulaganja u sektor reciklaže plastike.

        </p>

        <h4 class="text-xl font-semibold mb-4">
            Objavljena dokumenta
        </h4>

        <ol class="list-decimal ml-6 space-y-3 text-gray-700 mb-8">

            <li>
                Implementing Decision on the calculation,
                verification and reporting of data on recycled
                plastic content in single-use plastic beverage bottles
            </li>

            <li>
                Annexes to the Implementing Decision
            </li>

            <li>
                Staff Working Document
            </li>

        </ol>

        <h4 class="text-xl font-semibold mb-4">

            Stručni komentar GVP Consult

        </h4>

        <div class="bg-orange-50 border-l-4 border-orange-500 p-6 rounded">

            <p class="text-gray-700">

                Nova metodologija predstavlja važan korak ka većoj
                transparentnosti u oblasti reciklirane plastike.

                Privredni subjekti koji proizvode ili stavljaju PET
                ambalažu na tržište trebalo bi da na vreme prilagode
                svoje procedure i dokumentaciju kako bi ispunili
                nove regulatorne zahteve.

            </p>

        </div>

        <div class="mt-8">

            <a
                href="https://environment.ec.europa.eu/publications/implementing-decision-calculation-verification-and-reporting-data-recycled-plastic-content-single_en"
                target="_blank"
                class="inline-flex items-center text-orange-600 font-semibold hover:underline"
            >
                Zvanična dokumentacija Evropske komisije →
            </a>

        </div>

    </div>

</article>

</template>