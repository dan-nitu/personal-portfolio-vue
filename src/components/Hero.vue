<script setup>
import MapPinIcon from './icons/MapPinIcon.vue';
import GithubMarkWhiteIcon from './icons/GithubMarkWhiteIcon.vue';
import LinkedinLogoIcon from './icons/LinkedinLogoIcon.vue';
</script>

<template>
  <section class="hero">
    <h1>Hi, I'm Dan 👋</h1>

    <div>
      <h4>
        I'm a web developer focused on frontend technologies, with experience in
        PHP and Vue.js.
      </h4>
    </div>

    <div class="wrapper">
      <div class="location"><MapPinIcon /> Cluj-Napoca, Cluj, Romania</div>

      <div class="socials">
        <a
          href="https://github.com/dan-nitu"
          target="_blank"
          rel="noopener noreferrer"
        >
          <GithubMarkWhiteIcon
        /></a>
        <a href="https://www.linkedin.com/in/dan-nitu/" target="_blank">
          <LinkedinLogoIcon
        /></a>
      </div>
    </div>
  </section>
</template>
