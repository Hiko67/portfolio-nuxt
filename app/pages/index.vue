
<template>
  <section class="hero min-h-[75vh] bg-base-200">
    <div class="hero-content text-center">
      <div class="max-w-2xl">
        <h1 class="text-4xl font-bold md:text-6xl">
          Hi, I'm James Magpali
        </h1>

        <p class="mt-6 text-lg">
          I'm an IT student interested in web development
          and cybersecurity.
        </p>

        <p class="mt-4 text-base-content/70">
          Welcome to my portfolio, where I share my
          skills, projects, and certifications.
        </p>

        <div class="mt-8 flex justify-center gap-3">
          <NuxtLink to="/about" class="btn btn-primary">
            About Me
          </NuxtLink>

          <NuxtLink to="/contact" class="btn btn-outline">
            Contact Me
          </NuxtLink>
        </div>
      </div>
    </div>
  </section>
</template>
