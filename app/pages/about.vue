
<template>
  <section class="min-h-screen bg-base-200 px-6 py-16">
    <div class="mx-auto max-w-5xl">
      <h1 class="mb-4 text-center text-4xl font-bold">
        About Me
      </h1>

      <p class="mb-10 text-center text-base-content/70">
        Get to know more about me, my background, and my goals.
      </p>

      <div class="grid gap-6 md:grid-cols-2">
        <div class="card bg-base-100 shadow-md">
          <div class="card-body">
            <h2 class="card-title">Who I Am</h2>
            <p>
              Hi! I'm James Andrei Magpali, an Information
              Technology student with an interest in web
              development and cybersecurity.
            </p>
            <p class="mt-3">
              I enjoy learning new technologies and improving
              my programming skills through projects.
            </p>
          </div>
        </div>

        <div class="card bg-base-100 shadow-md">
          <div class="card-body">
            <h2 class="card-title">My Goals</h2>
            <p>
              My goal is to continue developing my technical
              skills and gain more experience in the IT field.
            </p>
            <p class="mt-3">
              I'm particularly interested in understanding
              how applications work and how to keep
              systems secure.
            </p>
          </div>
        </div>
      </div>

      <div class="mt-10 text-center">
        <NuxtLink to="/tech-stack" class="btn btn-primary">
          View My Tech Stack
        </NuxtLink>
      </div>
    </div>
  </section>
</template>
