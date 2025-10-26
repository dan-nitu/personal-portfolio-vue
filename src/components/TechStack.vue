<script setup>
import Frontend from './tech-stack-and-skills/Frontend.vue';
import Backend from './tech-stack-and-skills/Backend.vue';
import HostingTools from './tech-stack-and-skills/HostingTools.vue';
import OperatingSystems from './tech-stack-and-skills/OperatingSystems.vue';
import VersionControl from './tech-stack-and-skills/VersionControl.vue';
import TaskManagement from './tech-stack-and-skills/TaskManagement.vue';
import OtherTools from './tech-stack-and-skills/OtherTools.vue';
</script>

<template>
  <div class="tech-stack" id="tech-stack">
    <h2>Tech Stack 'n' Skills</h2>

    <div class="cards-wrapper">
      <Frontend />
      <Backend />
      <HostingTools />
      <OperatingSystems />
      <VersionControl />
      <TaskManagement />
      <OtherTools />
    </div>
  </div>
</template>
