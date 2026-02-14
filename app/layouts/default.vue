<script setup lang="ts">
import { cn } from '@/lib/utils'

const route = useRoute()
const isLayoutScrollDisabled = computed(() => route.meta.disableLayoutScroll === true)
</script>

<template>
  <SidebarProvider>
    <LayoutAppSidebar />
    <SidebarInset
      :class="cn(
        'flex flex-col h-screen',
        !isLayoutScrollDisabled && 'overflow-y-auto'
      )"
    >
      <LayoutHeader />
      <div class="flex flex-col flex-1">
        <div class="@container/main p-4 lg:p-6 grow">
          <slot />
        </div>
      </div>
    </SidebarInset>
  </SidebarProvider>
</template>

<style scoped>

</style>
