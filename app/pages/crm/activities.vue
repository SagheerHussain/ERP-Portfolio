<script setup lang="ts">
</script>

<template>
  <ErpModulePage
    title="Activities"
    description="Log and track all customer-facing activities including calls, meetings, emails, and tasks across your entire team."
    icon="i-lucide-activity"
    status="available"
    :stats="[
      { label: 'This Week', value: '342' },
      { label: 'Calls Made', value: '128' },
      { label: 'Meetings', value: '47' },
      { label: 'Emails Sent', value: '891' },
    ]"
    :features="[
      { title: 'Activity Feed', description: 'Real-time feed of all team activities with filtering by type, rep, account, and date range.', icon: 'i-lucide-rss' },
      { title: 'Call Logging', description: 'One-click call logging with duration tracking, notes, outcomes, and automatic contact association.', icon: 'i-lucide-phone' },
      { title: 'Meeting Scheduler', description: 'Calendar integration with availability sharing, room booking, and automated meeting follow-ups.', icon: 'i-lucide-calendar' },
      { title: 'Task Automation', description: 'Create recurring tasks, set follow-up reminders, and automate task assignment based on triggers.', icon: 'i-lucide-bot' },
      { title: 'Performance Metrics', description: 'Track activity volume, outcomes, and conversion rates per team member and account.', icon: 'i-lucide-gauge' },
      { title: 'Email Integration', description: 'Two-way email sync with automatic logging, template management, and open tracking.', icon: 'i-lucide-mail-check' },
    ]"
  />
</template>
