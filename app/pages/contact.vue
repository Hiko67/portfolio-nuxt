
<script setup lang="ts">
const contacts = [
  {
    name: 'GitHub',
    description: 'Explore my projects and repositories.',
    url: 'https://github.com/Hiko67'
  },
  {
    name: 'Facebook',
    description: 'Connect with me on Facebook.',
    url: 'https://www.facebook.com/dray2838288382'
  },
  {
    name: 'LinkedIn',
    description: 'Connect with me professionally on LinkedIn.',
    url: 'https://www.linkedin.com/in/andrei-magpali/'
  }
]
</script>


<template>
  <section class="min-h-screen bg-base-200 px-6 py-16">
    <div class="mx-auto max-w-5xl">
      <h1 class="text-center text-4xl font-bold">
        Contact Me
      </h1>

      <p class="mt-4 text-center text-base-content/70">
        Feel free to connect with me and explore my work.
      </p>

      <div class="mx-auto mt-10 max-w-md space-y-4">
        <div
          v-for="contact in contacts"
          :key="contact.name"
          class="card bg-base-100 shadow-md"
        >
          <div class="card-body">
            <h2 class="card-title">
              {{ contact.name }}
            </h2>

            <p class="text-base-content/70">
              {{ contact.description }}
            </p>

            <div class="card-actions mt-4 justify-end">
              <a
                :href="contact.url"
                target="_blank"
                rel="noopener noreferrer"
                class="btn btn-primary"
              >
                Visit Profile
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
