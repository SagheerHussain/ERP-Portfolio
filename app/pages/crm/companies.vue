<script setup lang="ts">
</script>

<template>
  <ErpModulePage
    title="Companies"
    description="Manage your B2B accounts with hierarchical company structures, financial data, and relationship mapping across your portfolio."
    icon="i-lucide-building-2"
    status="available"
    :stats="[
      { label: 'Total Companies', value: '612' },
      { label: 'Enterprise', value: '89' },
      { label: 'Active Contracts', value: '234' },
      { label: 'Total Revenue', value: '$4.8M' },
    ]"
    :features="[
      { title: 'Account Hierarchies', description: 'Map parent-child company relationships with subsidiary tracking and consolidated financial views.', icon: 'i-lucide-network' },
      { title: 'Financial Overview', description: 'Track revenue, outstanding invoices, payment history, and lifetime value per account.', icon: 'i-lucide-wallet' },
      { title: 'Stakeholder Mapping', description: 'Identify key decision-makers, influencers, and champions within each organization.', icon: 'i-lucide-users' },
      { title: 'Industry Classification', description: 'Categorize companies by industry, size, region, and custom attributes for strategic segmentation.', icon: 'i-lucide-filter' },
      { title: 'Contract Management', description: 'Track active contracts, renewal dates, and SLA compliance for each account.', icon: 'i-lucide-file-check' },
      { title: 'Account Health Score', description: 'Automated health scoring based on engagement, support tickets, and revenue trends.', icon: 'i-lucide-heart-pulse' },
    ]"
  />
</template>
