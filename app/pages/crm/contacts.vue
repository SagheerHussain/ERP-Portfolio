<script setup lang="ts">
</script>

<template>
  <ErpModulePage
    title="Contacts"
    description="Manage all your business contacts, track interactions, and build stronger relationships with centralized contact management."
    icon="i-lucide-contact"
    status="available"
    :stats="[
      { label: 'Total Contacts', value: '2,847' },
      { label: 'Active', value: '1,923' },
      { label: 'New This Month', value: '156' },
      { label: 'Avg. Response Time', value: '2.4h' },
    ]"
    :features="[
      { title: 'Smart Contact Cards', description: 'Rich contact profiles with full interaction history, notes, tags, and custom fields for comprehensive relationship tracking.', icon: 'i-lucide-id-card' },
      { title: 'Segmentation & Tags', description: 'Organize contacts with intelligent tagging, custom segments, and dynamic lists for targeted communication.', icon: 'i-lucide-tags' },
      { title: 'Import & Sync', description: 'Bulk import from CSV, Excel, or connect with third-party services like Google Contacts and Outlook.', icon: 'i-lucide-refresh-cw' },
      { title: 'Activity Timeline', description: 'Complete chronological timeline of every email, call, meeting, and note associated with each contact.', icon: 'i-lucide-history' },
      { title: 'Duplicate Detection', description: 'AI-powered duplicate detection and merge capabilities to keep your database clean and accurate.', icon: 'i-lucide-scan-search' },
      { title: 'Communication Hub', description: 'Send emails, schedule calls, and manage follow-ups directly from the contact record.', icon: 'i-lucide-message-square' },
    ]"
  />
</template>
