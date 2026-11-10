
<script setup lang="ts">
defineProps<{
  name: string
  category: string
  description: string
}>()
</script>

<template>
  <div class="card bg-base-100 shadow-md">
    <div class="card-body">
      <h2 class="card-title">{{ name }}</h2>

      <div class="badge badge-primary">
        {{ category }}
      </div>

      <p class="mt-3 text-base-content/70">
        {{ description }}
      </p>
    </div>
  </div>
</template>
