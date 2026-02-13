<script setup lang="ts">
</script>

<template>
  <ErpModulePage
    title="Invoices"
    description="Generate, send, and track invoices with automated payment reminders, multi-currency support, and accounting integration."
    icon="i-lucide-receipt"
    status="available"
    :stats="[
      { label: 'Outstanding', value: '$124K' },
      { label: 'Paid This Month', value: '$348K' },
      { label: 'Overdue', value: '$18.2K' },
      { label: 'Avg. Collection', value: '14 days' },
    ]"
    :features="[
      { title: 'Auto-Generation', description: 'Automatically generate invoices from orders, contracts, or time entries with configurable billing cycles.', icon: 'i-lucide-wand-2' },
      { title: 'Payment Tracking', description: 'Real-time payment status tracking with partial payment support and payment plan management.', icon: 'i-lucide-credit-card' },
      { title: 'Smart Reminders', description: 'Automated payment reminders with escalation rules based on aging tiers and client history.', icon: 'i-lucide-bell' },
      { title: 'PDF Generation', description: 'Professional PDF invoices with custom branding, multiple templates, and automatic email delivery.', icon: 'i-lucide-file-output' },
      { title: 'Tax Compliance', description: 'Region-specific tax calculation with GST, VAT, and sales tax support for global operations.', icon: 'i-lucide-shield-check' },
      { title: 'Recurring Billing', description: 'Set up recurring invoices for subscriptions and retainers with automatic charge processing.', icon: 'i-lucide-repeat' },
    ]"
  />
</template>
