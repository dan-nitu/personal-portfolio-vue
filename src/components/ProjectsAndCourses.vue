<script setup>
import Projects from './projects-and-courses/Projects.vue';
import Courses from './projects-and-courses/Courses.vue';
import OtherProjects from './projects-and-courses/OtherProjects.vue';
</script>

<template>
  <section class="projects-and-courses" id="projects">
    <h2>Projects 'n' Courses</h2>

    <div class="categories-wrapper">
      <Projects />
      <Courses />
      <OtherProjects />
    </div>
  </section>
</template>
