
<script setup lang="ts">
const personalInfo = [
  { label: 'Full Name', value: 'Richelle Ann W. Calabroso' },
  { label: 'Course', value: 'BS Information Technology' },
  { label: 'Age', value: '20 years old' },
  { label: 'Year Level', value: 'Third Year' },
  { label: 'University', value: 'Caraga State University' }
]

const education = [
  {
    level: 'College',
    school: 'Caraga State University',
    program: 'BS Information Technology'
  },
  {
    level: 'Senior High School',
    school: 'Agusan National High School',
    program: 'Humanities and Social Sciences (HUMSS)'
  },
  {
    level: 'Junior High School',
    school: 'Agusan National High School',
    program: 'Junior High School'
  },
  {
    level: 'Elementary',
    school: 'Silad Mahogany Elementary School',
    program: 'Elementary Education'
  }
]

const skills = [
  {
    title: 'Python Programming',
    description: 'Programming activities using Python'
  },
  {
    title: 'Web Development',
    description: 'Frontend development and Nuxt'
  },
  {
    title: 'Database Management',
    description: 'SQL and PostgreSQL'
  },
  {
    title: 'Computer Networking',
    description: 'Networking fundamentals and LAN practice'
  },
  {
    title: 'Microsoft Office',
    description: 'Working with Office applications'
  },
  {
    title: 'UI Design and Prototyping',
    description: 'Creating designs using Figma'
  }
]

const hobbies = [
  {
    title: 'Reading Stories',
    description: 'I enjoy reading novels and online stories, especially fantasy and world-hopping stories.',
    symbol: '01'
  },
  {
    title: 'Watching Movies and Series',
    description: 'I enjoy watching movies and television series with interesting characters and storylines.',
    symbol: '02'
  },
  {
    title: 'Watching Documentaries',
    description: 'I am interested in documentaries, particularly those about psychology and human behavior.',
    symbol: '03'
  },
  {
    title: 'Relaxing at Home',
    description: 'I appreciate quiet moments and enjoy spending my free time in the comfort of home.',
    symbol: '04'
  }
]
</script>

<template>
  <main class="min-h-screen bg-[#F7F3EC] text-[#263B50]">

    <div class="mx-auto max-w-6xl px-6 py-16 md:px-10">

      <!-- Page Heading -->
      <div class="mb-14 text-center">
        <p class="text-sm font-semibold uppercase tracking-[0.22em] text-[#B58A4B]">
          Get to know me
        </p>

        <h1 class="mt-3 text-4xl font-semibold tracking-tight text-[#263B50] md:text-5xl">
          About Me
        </h1>

        <p class="mt-4 text-[#6F8FA8]">
          A little more about my background and experiences.
        </p>
      </div>

      <!-- About Me -->
      <section class="mb-16 rounded-2xl border border-[#D8C8B5] bg-white p-7 shadow-sm md:p-10">

        <div class="mb-5 flex items-center gap-3">
          <div class="h-8 w-1 rounded-full bg-[#B58A4B]"></div>

          <h2 class="text-2xl font-semibold text-[#263B50]">
            Who I Am
          </h2>
        </div>

        <p class="max-w-4xl text-base leading-8 text-[#5F6265]">
          Hi! I'm Richelle Ann W. Calabroso, a third-year BS Information Technology student at Caraga State University. My college journey has been filled with new experiences, challenges, and lessons, but one of the things I appreciate most is the people I've met along the way. Through friendships, shared laughter, group activities, and even stressful school days, I've made memories that have made my time in college more meaningful. Alongside these experiences, I've also been introduced to different areas of technology and continue to learn as I move forward in my studies.
        </p>

      </section>

      <!-- Personal Information and Education -->
      <section class="mb-16">

        <div class="mb-8">
          <p class="text-sm font-semibold uppercase tracking-[0.2em] text-[#B58A4B]">
            My Background
          </p>

          <h2 class="mt-2 text-3xl font-semibold text-[#263B50]">
            Personal Information
          </h2>
        </div>

        <div class="grid items-stretch gap-8 md:grid-cols-2">

          <!-- Personal Information -->
          <div class="h-full rounded-2xl border border-[#D8C8B5] bg-white p-7 shadow-sm">

            <h3 class="mb-6 text-xl font-semibold text-[#263B50]">
              Personal Details
            </h3>

            <div class="flex flex-col justify-between gap-6 md:min-h-[420px]">
              <div
                v-for="item in personalInfo"
                :key="item.label"
                class="border-b border-[#EAE3D9] pb-4 last:border-0 last:pb-0"
              >
                <p class="text-xs font-semibold uppercase tracking-wider text-[#6F8FA8]">
                  {{ item.label }}
                </p>

                <p class="mt-1 font-medium text-[#263B50]">
                  {{ item.value }}
                </p>
              </div>
            </div>

          </div>

          <!-- Educational Background -->
          <div class="h-full rounded-2xl border border-[#D8C8B5] bg-white p-7 shadow-sm">

            <h3 class="mb-6 text-xl font-semibold text-[#263B50]">
              Educational Background
            </h3>

            <div class="space-y-8">
              <div
                v-for="item in education"
                :key="item.level"
                class="relative border-l-2 border-[#B58A4B] pl-5"
              >
                <p class="text-xs font-semibold uppercase tracking-wider text-[#6F8FA8]">
                  {{ item.level }}
                </p>

                <h4 class="mt-2 text-lg font-semibold text-[#263B50]">
                  {{ item.school }}
                </h4>

                <p class="mt-1 text-sm text-[#5F6265]">
                  {{ item.program }}
                </p>
              </div>
            </div>

          </div>

        </div>
      </section>

      <!-- Skills and Interests -->
      <section class="mb-16">

        <div class="mb-8">
          <p class="text-sm font-semibold uppercase tracking-[0.2em] text-[#B58A4B]">
            What I've learned
          </p>

          <h2 class="mt-2 text-3xl font-semibold text-[#263B50]">
            Skills and Interests
          </h2>

          <p class="mt-3 max-w-2xl leading-7 text-[#5F6265]">
            Different areas of technology and tools I've been introduced to through my studies and academic activities.
          </p>
        </div>

        <div class="grid gap-4 sm:grid-cols-2 lg:grid-cols-3">

          <div
            v-for="(skill, index) in skills"
            :key="skill.title"
            class="rounded-xl border border-[#D8C8B5] bg-white p-6 transition duration-300 hover:-translate-y-1 hover:shadow-md"
          >
            <p class="text-sm font-semibold tracking-widest text-[#B58A4B]">
              0{{ index + 1 }}
            </p>

            <h3 class="mt-4 text-lg font-semibold text-[#263B50]">
              {{ skill.title }}
            </h3>

            <p class="mt-2 text-sm leading-6 text-[#66736D]">
              {{ skill.description }}
            </p>
          </div>

        </div>
      </section>

      <!-- Hobbies -->
      <section class="mb-16">

        <div class="mb-8">
          <p class="text-sm font-semibold uppercase tracking-[0.2em] text-[#B58A4B]">
            Outside academics
          </p>

          <h2 class="mt-2 text-3xl font-semibold text-[#263B50]">
            My Hobbies
          </h2>

          <p class="mt-3 max-w-2xl leading-7 text-[#5F6265]">
            Things I enjoy doing during my free time.
          </p>
        </div>

        <div class="grid gap-5 sm:grid-cols-2">

          <div
            v-for="hobby in hobbies"
            :key="hobby.title"
            class="flex gap-5 rounded-2xl border border-[#D8C8B5] bg-white p-6 shadow-sm"
          >
            <div class="flex h-12 w-12 shrink-0 items-center justify-center rounded-full bg-[#F7F3EC] text-sm font-semibold text-[#B58A4B]">
              {{ hobby.symbol }}
            </div>

            <div>
              <h3 class="text-lg font-semibold text-[#263B50]">
                {{ hobby.title }}
              </h3>

              <p class="mt-2 text-sm leading-7 text-[#66736D]">
                {{ hobby.description }}
              </p>
            </div>
          </div>

        </div>
      </section>

      <!-- Back to Home -->
      <div class="text-center">
        <NuxtLink
          to="/"
          class="inline-flex items-center gap-3 rounded-full bg-[#263B50] px-8 py-3.5 text-sm font-medium text-white transition duration-300 hover:bg-[#6F8FA8]"
        >
          <span>←</span>
          Back to Home
        </NuxtLink>
      </div>

    </div>
  </main>
</template>
