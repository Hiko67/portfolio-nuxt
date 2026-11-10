
<script setup lang="ts">
defineProps<{
  title: string
  issuer: string
  description: string
}>()
</script>

<template>
  <div class="card bg-base-100 shadow-md">
    <div class="card-body">
      <h2 class="card-title">{{ title }}</h2>

      <div class="badge badge-primary">
        {{ issuer }}
      </div>

      <p class="mt-4 text-base-content/70">
        {{ description }}
      </p>
    </div>
  </div>
</template>
