<script setup>
import CPanelLogoIcon from '@/components/icons/CPanelLogoIcon.vue';
import VercelLogoIcon from '@/components/icons/VercelLogoIcon.vue';
import NetlifyLogoIcon from '@/components/icons/NetlifyLogoIcon.vue';
</script>

<template>
  <div class="card">
    <div class="card-heading">Hosting tools</div>
    <div class="showcase">
      <div>
        <CPanelLogoIcon />
        <span>cPanel</span>
      </div>
      <div>
        <VercelLogoIcon />
        <span>Vercel</span>
      </div>
      <div>
        <NetlifyLogoIcon />
        <span>Netlify</span>
      </div>
    </div>
  </div>
</template>
