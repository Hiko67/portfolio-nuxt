
<script setup lang="ts">
const links = [
  { label: 'Home', to: '/' },
  { label: 'About', to: '/about' },
  { label: 'Tech Stack', to: '/tech-stack' },
  { label: 'Certifications', to: '/certifications' },
  { label: 'Contact', to: '/contact' }
]
</script>

<template>
  <header class="bg-base-100 shadow-sm">
    <nav class="navbar mx-auto max-w-6xl px-4">
      <div class="navbar-start">
        <NuxtLink to="/" class="btn btn-ghost text-xl font-bold">
          James Magpali
        </NuxtLink>
      </div>

      <!-- Desktop navigation -->
      <div class="navbar-end hidden lg:flex">
        <ul class="menu menu-horizontal gap-1 px-1">
          <li v-for="link in links" :key="link.to">
            <NuxtLink :to="link.to">
              {{ link.label }}
            </NuxtLink>
          </li>
        </ul>
      </div>

      <!-- Mobile navigation -->
      <div class="navbar-end lg:hidden">
        <details class="dropdown dropdown-end">
          <summary class="btn btn-ghost" aria-label="Open navigation menu">
            Menu
          </summary>

          <ul class="menu dropdown-content bg-base-100 rounded-box z-50 mt-3 w-52 p-2 shadow-lg">
            <li v-for="link in links" :key="link.to">
              <NuxtLink :to="link.to">
                {{ link.label }}
              </NuxtLink>
            </li>
          </ul>
        </details>
      </div>
    </nav>
  </header>
</template>
