<template>
  <div class="w-full max-w-screen-lg block mx-auto p-4">
    <div class="grid grid-cols-12 gap-3">
      <div class="hidden md:block col-span-4">
        <UNavigationMenu orientation="vertical" :items="items" class="data-[orientation=vertical]:w-full" />
      </div>

      <div class="col-span-12 md:col-span-8">
        Chat
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import type { NavigationMenuItem } from '@nuxt/ui'

const items = ref<NavigationMenuItem[][]>([
  [
    {
      label: 'Select User',
      type: 'label'
    },
    {
      label: 'Kiran Sai Subramanyam K',
      avatar: {
        alt: 'User',
        src: 'https://github.com/benjamincanac.png'
      }
    }
  ]
])
</script>