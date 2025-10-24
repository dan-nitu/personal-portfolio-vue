<script setup>
import AzureDevOpsLogoIcon from '@/components/icons/AzureDevOpsLogoIcon.vue';
import JiraLogoIcon from '@/components/icons/JiraLogoIcon.vue';
import AsanaLogoIcon from '@/components/icons/AsanaLogoIcon.vue';
import TrelloLogoIcon from '@/components/icons/TrelloLogoIcon.vue';
</script>

<template>
  <div class="card">
    <div class="card-heading">Task Management & Agile methodology</div>
    <div class="showcase">
      <div>
        <AzureDevOpsLogoIcon />
        <span>Azure DevOps</span>
      </div>
      <div>
        <JiraLogoIcon />
        <span>Jira</span>
      </div>
      <div>
        <AsanaLogoIcon />
        <span>Asana</span>
      </div>
      <div>
        <TrelloLogoIcon />
        <span>Trello</span>
      </div>
    </div>
  </div>
</template>
