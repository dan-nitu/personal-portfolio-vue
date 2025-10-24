<script setup>
import MicrosoftWindowsLogoIcon from '@/components/icons/MicrosoftWindowsLogoIcon.vue';
import UbuntuLogoIcon from '@/components/icons/UbuntuLogoIcon.vue';
import MacOSLogoIcon from '@/components/icons/MacOSLogoIcon.vue';
</script>

<template>
  <div class="card">
    <div class="card-heading">Operating Systems</div>
    <div class="showcase">
      <div>
        <MicrosoftWindowsLogoIcon />
        <span>Microsoft Windows</span>
      </div>
      <div>
        <UbuntuLogoIcon />
        <span>Linux (Ubuntu)</span>
      </div>
      <div>
        <MacOSLogoIcon />
        <span>macOS</span>
      </div>
    </div>
  </div>
</template>
