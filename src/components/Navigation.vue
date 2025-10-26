<script setup>
import { ref, watch, onBeforeUnmount } from 'vue';

const isNavOpen = ref(false);

const closeNav = () => {
  isNavOpen.value = false;
};

const scrollToSection = (sectionId) => {
  const target = document.getElementById(sectionId);
  const offset = 55;
  if (target) {
    const targetPosition =
      target.getBoundingClientRect().top + window.pageYOffset;
    window.scrollTo({
      top: targetPosition - offset,
      behavior: 'smooth',
    });
  }

  closeNav();
};

const scrollToTop = () => {
  window.scrollTo({
    top: 0,
    behavior: 'smooth',
  });
  closeNav();
};

watch(isNavOpen, (newState) => {
  if (newState) {
    document.body.style.overflow = 'hidden';
  } else {
    document.body.style.overflow = '';
  }
});

onBeforeUnmount(() => {
  document.body.style.overflow = '';
});
</script>

<template>
  <nav>
    <input type="checkbox" id="toggler" v-model="isNavOpen" name="toggler" />
    <label for="toggler"></label>

    <span @click="scrollToTop"> DanNițu </span>

    <ul>
      <li>
        <a href="#about" @click.prevent="scrollToSection('about')">About</a>
      </li>
      <li>
        <a href="#tech-stack" @click.prevent="scrollToSection('tech-stack')"
          >Tech Stack</a
        >
      </li>
      <li>
        <a href="#experience" @click.prevent="scrollToSection('experience')"
          >Experience</a
        >
      </li>
      <li>
        <a href="#projects" @click.prevent="scrollToSection('projects')"
          >Projects</a
        >
      </li>
    </ul>
  </nav>
</template>
