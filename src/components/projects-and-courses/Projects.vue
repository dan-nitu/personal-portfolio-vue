<script setup>
import weatherNow from '@/assets/images/projects/weather-now.png';
import spaceTourismWebsite from '@/assets/images/projects/space-tourism-website.png';
import rockPaperScissors from '@/assets/images/projects/rock-paper-scissors.png';
import countriesApp from '@/assets/images/projects/countries-app.png';
import weatherApp from '@/assets/images/projects/weather-app.png';

const projects = [
  {
    id: 1,
    title: 'Weather Now',
    description: '(A Frontend Mentor challenge)',
    technology: 'vuejs',
    screenshot: weatherNow,
    demo: 'https://frontend-mentor-weather-now-app.vercel.app/',
    github: 'https://github.com/dan-nitu/frontend-mentor-weather-now-app',
  },
  {
    id: 2,
    title: 'Space Tourism Website',
    description: '(A Frontend Mentor challenge)',
    technology: 'html',
    screenshot: spaceTourismWebsite,
    demo: 'https://dn-space-tourism-website.vercel.app/',
    github: 'https://github.com/dan-nitu/space-tourism-website/tree/main',
  },
  {
    id: 3,
    title: 'Rock Paper Scissors',
    description: '(A Frontend Mentor challenge)',
    technology: 'javascript',
    screenshot: rockPaperScissors,
    demo: 'https://dn-js-rock-paper-scissors.vercel.app/',
    github: 'https://github.com/dan-nitu/rock-paper-scissors',
  },
  {
    id: 4,
    title: 'Countries APP',
    description: '(A Frontend Mentor challenge)',
    technology: 'react',
    screenshot: countriesApp,
    demo: 'https://dn-react-countries-app.vercel.app/',
    github: 'https://github.com/dan-nitu/countries-app-react',
  },
  {
    id: 5,
    title: 'Weather APP',
    technology: 'react',
    screenshot: weatherApp,
    demo: 'https://dn-react-weather-app.vercel.app/',
    github: 'https://github.com/dan-nitu/weather-app-react',
  },
];
</script>

<template>
  <div class="projects">
    <h4>A collection of my personal web development projects.</h4>

    <div class="cards-wrapper">
      <div v-for="project in projects" :key="project.id" class="card">
        <img :src="project.screenshot" :alt="project.title" />
        <span :class="`technology ${project.technology}`"></span>

        <div class="card-body">
          <h5>
            {{ project.title }}
          </h5>

          <p v-if="project.description">{{ project.description }}</p>

          <div class="buttons-wrapper">
            <a
              :href="project.demo"
              class="demo"
              target="_blank"
              rel="noopener noreferrer"
              >Demo</a
            >
            <a
              :href="project.github"
              class="github"
              target="_blank"
              rel="noopener noreferrer"
              >Github</a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
