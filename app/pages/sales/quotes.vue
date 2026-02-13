<script setup lang="ts">
</script>

<template>
  <ErpModulePage
    title="Quotes & Estimates"
    description="Create professional quotes and estimates with configurable line items, discount rules, and one-click conversion to invoices."
    icon="i-lucide-file-text"
    status="available"
    :stats="[
      { label: 'Active Quotes', value: '34' },
      { label: 'Total Value', value: '$287K' },
      { label: 'Accepted Rate', value: '68%' },
      { label: 'Avg. Turnaround', value: '1.8 days' },
    ]"
    :features="[
      { title: 'Template Builder', description: 'Drag-and-drop quote builder with reusable templates, custom branding, and dynamic pricing logic.', icon: 'i-lucide-layout-template' },
      { title: 'Line Item Management', description: 'Flexible line items with quantity tiers, bundled pricing, tax rules, and discount schedules.', icon: 'i-lucide-list' },
      { title: 'Approval Workflows', description: 'Multi-level approval chains for high-value quotes with notification escalation and audit trails.', icon: 'i-lucide-check-circle' },
      { title: 'E-Signatures', description: 'Built-in electronic signature collection for fast client approval without leaving the platform.', icon: 'i-lucide-pen-tool' },
      { title: 'Version Control', description: 'Track all quote revisions with change history and side-by-side comparison views.', icon: 'i-lucide-git-compare' },
      { title: 'Invoice Conversion', description: 'One-click conversion from accepted quote to invoice with all line items pre-populated.', icon: 'i-lucide-arrow-right' },
    ]"
  />
</template>
