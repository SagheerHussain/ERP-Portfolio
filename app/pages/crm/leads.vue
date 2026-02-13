<script setup lang="ts">
</script>

<template>
  <ErpModulePage
    title="Leads"
    description="Capture, qualify, and nurture leads through your sales pipeline with intelligent lead scoring and automated follow-ups."
    icon="i-lucide-magnet"
    status="available"
    :stats="[
      { label: 'Active Leads', value: '438' },
      { label: 'Qualified', value: '186' },
      { label: 'Conversion Rate', value: '23.4%' },
      { label: 'Avg. Deal Size', value: '$18.5K' },
    ]"
    :features="[
      { title: 'Lead Scoring', description: 'Automated lead scoring based on engagement, demographics, and behavioral data to prioritize high-value prospects.', icon: 'i-lucide-star' },
      { title: 'Pipeline Visualization', description: 'Visual pipeline stages with drag-and-drop progression and customizable qualification criteria.', icon: 'i-lucide-git-branch' },
      { title: 'Web Forms & Capture', description: 'Embed lead capture forms on your website with automatic CRM entry and assignment rules.', icon: 'i-lucide-layout' },
      { title: 'Lead Assignment', description: 'Round-robin or rule-based lead assignment to sales reps with territory and capacity management.', icon: 'i-lucide-user-plus' },
      { title: 'Nurture Campaigns', description: 'Automated drip campaigns and follow-up sequences based on lead behavior and engagement signals.', icon: 'i-lucide-sprout' },
      { title: 'Source Tracking', description: 'Track lead sources (organic, paid, referral) with ROI analysis per channel for optimized marketing spend.', icon: 'i-lucide-radar' },
    ]"
  />
</template>
