<template>
  <section id="contact" class="py-20 bg-[#f8f5f1]">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-12">
      <div>
        <span class="uppercase text-orange-500 text-sm tracking-widest">
          Kontakt
        </span>

        <h2 class="text-4xl font-serif font-bold mt-4 mb-6 text-[#222222]">
          Zakažite konsultacije
        </h2>

        <p class="text-gray-700 leading-relaxed mb-8">
          Za dodatne informacije, saradnju ili zakazivanje konsultacija,
          možete nas kontaktirati putem forme ili dostupnih kontakt podataka.
        </p>

        <div class="space-y-4 text-gray-700">
          <p><strong>Email:</strong> gvpconsult24@gmail.com</p>
          <p><strong>Telefon:</strong> +381 64 157 95 99</p>
          <p><strong>Lokacija:</strong> Srbija</p>
        </div>
      </div>

      <form class="bg-white p-8 rounded-lg shadow space-y-5">
        <input class="w-full border p-3 rounded" type="text" placeholder="Ime i prezime" />
        <input class="w-full border p-3 rounded" type="email" placeholder="Email adresa" />
        <input class="w-full border p-3 rounded" type="text" placeholder="Naslov poruke" />
        <textarea class="w-full border p-3 rounded h-36" placeholder="Vaša poruka"></textarea>

        <button class="bg-orange-500 hover:bg-orange-600 text-white px-7 py-3 rounded">
          Pošaljite poruku
        </button>
      </form>
    </div>
  </section>
</template>