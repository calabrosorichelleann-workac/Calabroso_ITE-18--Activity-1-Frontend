
<template>
  <header class="border-b border-[#6F8FA8] bg-[#263B50]">
    <nav class="mx-auto flex max-w-6xl items-center justify-between px-6 py-5 md:px-10">

      <!-- Website Name -->
      <NuxtLink
        to="/"
        class="text-xl font-semibold tracking-tight text-white transition-colors hover:text-[#B7C9D5]"
      >
        Richelle Ann<span class="text-[#B58A4B]">✦</span>
      </NuxtLink>

      <!-- Navigation Links -->
        <div class="flex items-center gap-7 text-base font-medium">

        <NuxtLink
          to="/"
          exact-active-class="!text-[#B58A4B]"
          class="text-white transition-colors hover:text-[#B7C9D5]"
        >
          Home
        </NuxtLink>

        <NuxtLink
          to="/profile"
          exact-active-class="!text-[#B58A4B]"
          class="text-white transition-colors hover:text-[#B7C9D5]"
        >
          Profile
        </NuxtLink>

      </div>
    </nav>
  </header>
</template>
