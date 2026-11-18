
<template>
  <div class="flex min-h-screen flex-col bg-[#F7F3EC]">

    <Nav />

    <div class="flex-1">
      <slot />
    </div>

    <footer class="border-t border-[#D8C8B5] px-6 py-5 text-center">
      <p class="text-sm text-[#526779]">
        © 2026 Richelle Ann | My Personal Website
      </p>
    </footer>

  </div>
</template>
