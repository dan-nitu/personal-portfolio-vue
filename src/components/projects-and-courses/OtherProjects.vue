<script setup>
import houseMarketplace from '@/assets/images/projects/house-marketplace.PNG';
import githubFinder from '@/assets/images/projects/github-finder.png';
import weatherJS from '@/assets/images/projects/weatherjs.PNG';
import userForm from '@/assets/images/projects/user-form.PNG';
import tracalorie from '@/assets/images/projects/tracalorie.PNG';
import tasklist from '@/assets/images/projects/task-list.PNG';
import profileScroller from '@/assets/images/projects/profile-scroller.PNG';
import numberGuesser from '@/assets/images/projects/number-guesser.PNG';
import loanCalculator from '@/assets/images/projects/loan-calculator.PNG';
import chuckNorrisJokes from '@/assets/images/projects/chuck-norris-jokes.PNG';
import booklist from '@/assets/images/projects/booklist.PNG';

const otherProjects = [
  {
    id: 1,
    title: 'House Marketplace',
    technology: 'react',
    screenshot: houseMarketplace,
    demo: 'https://dn-react-house-marketplace.vercel.app/',
    github:
      'https://github.com/dan-nitu/house-marketplace-react-front-to-back-2022',
  },
  {
    id: 2,
    title: 'Github Finder',
    technology: 'react',
    screenshot: githubFinder,
    demo: 'https://dn-react-github-finder.vercel.app/',
    github:
      'https://github.com/dan-nitu/github-finder-react-front-to-back-2022',
  },
  {
    id: 3,
    title: 'WeatherJS',
    technology: 'javascript',
    screenshot: weatherJS,
    demo: 'https://dn-js-weatherjs.vercel.app/',
    github: 'https://github.com/dan-nitu/weatherjs-mjsftb',
  },
  {
    id: 4,
    title: 'Userform',
    technology: 'javascript',
    screenshot: userForm,
    demo: 'https://dn-js-userform.vercel.app/',
    github: 'https://github.com/dan-nitu/userform-mjsftb',
  },
  {
    id: 5,
    title: 'Tracalorie',
    technology: 'javascript',
    screenshot: tracalorie,
    demo: 'https://dn-js-tracalorie.vercel.app/',
    github: 'https://github.com/dan-nitu/tracalorie-mjsftb',
  },
  {
    id: 6,
    title: 'Tasklist',
    technology: 'javascript',
    screenshot: tasklist,
    demo: 'https://dn-js-tasklist.vercel.app/',
    github: 'https://github.com/dan-nitu/tasklist-mjsftb',
  },
  {
    id: 7,
    title: 'Profile Scroller',
    technology: 'javascript',
    screenshot: profileScroller,
    demo: 'https://dn-js-profilescroller.vercel.app/',
    github: 'https://github.com/dan-nitu/profilescroller-mjsftb',
  },
  {
    id: 8,
    title: 'Number Guesser',
    technology: 'javascript',
    screenshot: numberGuesser,
    demo: 'https://dn-js-numberguesser.vercel.app/',
    github: 'https://github.com/dan-nitu/numberguesser-mjsftb',
  },
  {
    id: 9,
    title: 'Loan Calculator',
    technology: 'javascript',
    screenshot: loanCalculator,
    demo: 'https://dn-js-loancalculator.vercel.app/',
    github: 'https://github.com/dan-nitu/loancalculator-mjsftb',
  },
  {
    id: 10,
    title: 'Chuck Norris Jokes',
    technology: 'javascript',
    screenshot: chuckNorrisJokes,
    demo: 'https://dn-js-chucknorrisjokes.vercel.app/',
    github: 'https://github.com/dan-nitu/chucknorrisjokes-mjsftb',
  },
  {
    id: 11,
    title: 'Booklist',
    technology: 'javascript',
    screenshot: booklist,
    demo: 'https://dn-js-booklist.vercel.app/',
    github: 'https://github.com/dan-nitu/booklist-mjsftb',
  },
];
</script>

<template>
  <div class="other-projects">
    <h4>Other things I've built just for the love of it.</h4>

    <div class="cards-wrapper">
      <div v-for="project in otherProjects" :key="project.id" class="card">
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
              class="button demo"
              target="_blank"
              rel="noopener noreferrer"
              >Demo</a
            >
            <a
              :href="project.github"
              class="button github"
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
