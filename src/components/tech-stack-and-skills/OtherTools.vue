<script setup>
import BrowserstackLogoIcon from '@/components/icons/BrowserstackLogoIcon.vue';
import PostmanLogoIcon from '@/components/icons/PostmanLogoIcon.vue';
import FirebaseLogoIcon from '@/components/icons/FirebaseLogoIcon.vue';
import MongoDBCompassLogoIcon from '@/components/icons/MongoDBCompassLogoIcon.vue';
</script>

<template>
  <div class="card">
    <div class="card-heading">Other tools</div>
    <div class="showcase">
      <div>
        <BrowserstackLogoIcon />
        <span>Browserstack</span>
      </div>
      <div>
        <PostmanLogoIcon />
        <span>Postman</span>
      </div>
      <div>
        <FirebaseLogoIcon />
        <span>Firebase</span>
      </div>
      <div>
        <MongoDBCompassLogoIcon />
        <span>Mongo DB Compass</span>
      </div>
    </div>
  </div>
</template>
