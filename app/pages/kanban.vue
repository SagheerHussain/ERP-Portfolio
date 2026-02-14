<script setup lang="ts">
import KanbanBoard from '~/components/kanban/KanbanBoard.vue'

const { addColumn, resetBoard } = useKanban()

const showNewColumn = ref(false)
const newColumnTitle = ref('')

function createColumn() {
  if (!newColumnTitle.value.trim())
    return
  addColumn(newColumnTitle.value.trim())
  newColumnTitle.value = ''
  showNewColumn.value = false
}

function handleReset() {
  if (confirm('Reset board to include 100+ dummy records for performance testing?')) {
    resetBoard()
  }
}

definePageMeta({
  disableLayoutScroll: true,
})

const { setHeader } = usePageHeader()
setHeader({ title: 'Kanban Board', icon: 'i-lucide-kanban', description: 'Visual task management with drag-and-drop' })
</script>

<template>
  <div class="h-full flex flex-col overflow-hidden">
    <div class="flex flex-col gap-4 h-full min-h-0 overflow-hidden">
      <div class="flex items-center justify-end gap-2 shrink-0">
        <Button size="sm" variant="outline" @click="handleReset">
          <Icon name="i-lucide-refresh-cw" class="mr-1 size-4" />
          Reset to Demo
        </Button>
        <Button size="sm" @click="showNewColumn = true">
          <Icon name="lucide:plus" />
          Add Column
        </Button>
      </div>
      <KanbanBoard />
    </div>

    <!-- New Column Dialog -->
    <Dialog v-model:open="showNewColumn">
      <DialogContent class="sm:max-w-[420px]">
        <DialogHeader>
          <DialogTitle>Add New Column</DialogTitle>
          <DialogDescription class="sr-only">
            Add a new column to the board
          </DialogDescription>
        </DialogHeader>
        <form name="newColumnForm" class="flex flex-col gap-3" @submit.prevent="createColumn">
          <Input v-model="newColumnTitle" placeholder="Column title" />
        </form>
        <DialogFooter>
          <Button variant="secondary" @click="showNewColumn = false">
            Cancel
          </Button>
          <Button type="submit" form="newColumnForm" @click="createColumn">
            Create
          </Button>
        </DialogFooter>
      </DialogContent>
    </Dialog>
  </div>
</template>
