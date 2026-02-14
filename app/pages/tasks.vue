<script setup lang="ts">
definePageMeta({
  disableLayoutScroll: true,
})
import { columns } from '@/components/tasks/components/columns'
import DataTable from '@/components/tasks/components/DataTable.vue'
import tasks from '@/components/tasks/data/tasks.json'

const { setHeader } = usePageHeader()
setHeader({ title: 'Tasks', icon: 'i-lucide-calendar-check-2', description: 'Here\'s a list of your tasks for this month!' })
</script>

<template>
  <div class="w-full h-full flex flex-col items-stretch gap-4 overflow-hidden">
    <DataTable :data="tasks.data" :columns="columns" class="flex-1 min-h-0" />
  </div>
</template>

<style scoped>

</style>
