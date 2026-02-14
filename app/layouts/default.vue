<script setup lang="ts">
import { cn } from '@/lib/utils'

const route = useRoute()
const isLayoutScrollDisabled = computed(() => route.meta.disableLayoutScroll === true)
</script>

<template>
  <SidebarProvider
    :class="isLayoutScrollDisabled ? 'h-screen !min-h-0 overflow-hidden' : ''"
  >
    <LayoutAppSidebar />
    <SidebarInset
      :class="cn(
        'flex flex-col',
        isLayoutScrollDisabled ? 'h-screen overflow-hidden' : ''
      )"
    >
      <LayoutHeader />
      <div
        :class="cn(
          'flex flex-col flex-1 min-h-0',
          isLayoutScrollDisabled ? 'overflow-hidden' : 'overflow-y-auto'
        )"
      >
        <div
          :class="cn(
            '@container/main p-4 lg:p-6',
            isLayoutScrollDisabled ? 'flex-1 min-h-0 flex flex-col overflow-hidden' : 'grow'
          )"
        >
          <slot />
        </div>
      </div>
    </SidebarInset>
  </SidebarProvider>
</template>
