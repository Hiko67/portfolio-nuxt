
<script setup lang="ts">
const technologies = [
  {
    name: 'C',
    category: 'Programming',
    description: 'A programming language used for problem-solving and understanding programming fundamentals.'
  },
  {
    name: 'Java',
    category: 'Programming',
    description: 'An object-oriented programming language used to develop applications.'
  },
  {
    name: 'PostgreSQL',
    category: 'Database',
    description: 'A relational database system used to store and manage data.'
  },
  {
    name: 'HTML',
    category: 'Web Development',
    description: 'Used to structure the content of web pages.'
  },
  {
    name: 'CSS',
    category: 'Web Development',
    description: 'Used to style web pages and create responsive layouts.'
  },
  {
    name: 'Visual Studio Code',
    category: 'Development Tools',
    description: 'A code editor used for writing and managing projects.'
  },
  {
    name: 'Git',
    category: 'Development Tools',
    description: 'A version control tool used to track code changes.'
  },
  {
    name: 'GitHub',
    category: 'Development Tools',
    description: 'A platform for hosting repositories and managing code.'
  }
]
</script>

<template>
  <section class="min-h-screen bg-base-200 px-6 py-16">
    <div class="mx-auto max-w-6xl">
      <h1 class="text-center text-4xl font-bold">
        My Tech Stack
      </h1>

      <p class="mt-4 text-center text-base-content/70">
        Technologies and tools I have experience using.
      </p>

      <div class="mt-10 grid gap-6 sm:grid-cols-2 lg:grid-cols-3">
        <TechCard
          v-for="tech in technologies"
          :key="tech.name"
          :name="tech.name"
          :category="tech.category"
          :description="tech.description"
        />
      </div>
    </div>
  </section>
</template>
