<script setup lang="ts">
</script>

<template>
  <ErpModulePage
    title="Deals Pipeline"
    description="Track and manage deals through every stage of your sales cycle with visual pipelines, forecasting, and win/loss analysis."
    icon="i-lucide-handshake"
    status="beta"
    :stats="[
      { label: 'Open Deals', value: '67' },
      { label: 'Pipeline Value', value: '$1.2M' },
      { label: 'Won This Quarter', value: '$485K' },
      { label: 'Win Rate', value: '34.2%' },
    ]"
    :features="[
      { title: 'Visual Pipeline', description: 'Kanban-style deal boards with customizable stages, probability weights, and drag-and-drop management.', icon: 'i-lucide-kanban' },
      { title: 'Revenue Forecasting', description: 'AI-driven revenue forecasting based on pipeline velocity, historical win rates, and deal stage analytics.', icon: 'i-lucide-trending-up' },
      { title: 'Deal Rooms', description: 'Collaborative deal workspaces with shared documents, stakeholder mapping, and approval workflows.', icon: 'i-lucide-users' },
      { title: 'Proposal Builder', description: 'Generate professional proposals and quotes directly from deal records with template-based automation.', icon: 'i-lucide-file-plus' },
      { title: 'Win/Loss Analysis', description: 'Post-deal analysis with competitor tracking, loss reasons, and insights to improve future close rates.', icon: 'i-lucide-bar-chart' },
      { title: 'Multi-Currency', description: 'Handle international deals with real-time currency conversion and multi-currency pipeline views.', icon: 'i-lucide-coins' },
    ]"
  />
</template>
