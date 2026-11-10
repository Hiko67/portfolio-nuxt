
<script setup lang="ts">
const certifications = [
  {
    title: 'Python Essentials 1',
    issuer: 'Cisco',
    description: 'Learned Python programming fundamentals, including syntax, variables, loops, functions, and problem-solving.'
  },
  {
    title: 'IT Specialist Java',
    issuer: 'Certiport',
    description: 'Demonstrated knowledge of Java programming, object-oriented concepts, and application development.'
  },
  {
    title: 'Software Engineering',
    issuer: 'Saylor Academy',
    description: 'Studied software development processes, design principles, and software engineering fundamentals.'
  }
]
</script>

<template>
  <section class="min-h-screen bg-base-200 px-6 py-16">
    <div class="mx-auto max-w-6xl">
      <h1 class="text-center text-4xl font-bold">
        My Certifications
      </h1>

      <p class="mt-4 text-center text-base-content/70">
        Certifications and courses I have completed
        throughout my learning journey.
      </p>

      <div class="mt-10 grid gap-6 md:grid-cols-2 lg:grid-cols-3">
        <CertificationCard
          v-for="cert in certifications"
          :key="cert.title"
          :title="cert.title"
          :issuer="cert.issuer"
          :description="cert.description"
        />
      </div>
    </div>
  </section>
</template>
