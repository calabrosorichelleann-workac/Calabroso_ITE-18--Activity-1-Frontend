
<template>
  <main class="min-h-screen bg-[#F7F3EC] text-[#263B50]">

    <section class="mx-auto grid min-h-[85vh] max-w-6xl items-center gap-14 px-6 py-16 md:grid-cols-2 md:px-10">

      <!-- Introduction -->
      <div class="order-2 md:order-1">

        <p class="mb-6 text-base font-semibold uppercase tracking-[0.22em] text-[#B58A4B]">
           Hello, welcome!
        </p>

        <h1 class="text-5xl font-semibold tracking-tight text-[#263B50] md:text-6xl">
          I'm Richelle Ann.
        </h1>

        <p class="mt-6 text-lg font-medium leading-relaxed text-[#263B50]">
          Third-year BS Information Technology student at Caraga State University.
        </p>

        <div class="mt-7 max-w-xl space-y-5 text-base leading-8 text-[#5F6265]">
          <p>
            I'm learning more about Information Technology through my studies and the experiences that come with it. There is still much to understand, and I believe that each experience, whether big or small, has something to teach me.
          </p>

          <p>
            This website is a little introduction to who I am, what I study, and the things I enjoy. Feel free to explore and get to know me better!
          </p>
        </div>

        <!-- Profile Button -->
        <NuxtLink
          to="/profile"
          class="mt-9 inline-flex items-center gap-3 rounded-full bg-[#263B50] px-7 py-3.5 text-sm font-medium text-white transition duration-300 hover:bg-[#6F8FA8]"
        >
          Get to know me
          <span>→</span>
        </NuxtLink>

      </div>

      <!-- Profile Picture -->
      <div class="order-1 flex justify-center md:order-2 md:justify-end">
        <div class="relative w-full max-w-sm">

          <div class="absolute -bottom-3 -right-3 h-full w-full rounded-2xl border border-[#B58A4B]"></div>

          <img
            src="/images/profile.png"
            alt="Portrait of Richelle Ann"
            class="relative z-10 aspect-[4/5] w-full rounded-2xl object-cover shadow-lg"
          />

        </div>
      </div>

    </section>

  </main>
</template>
