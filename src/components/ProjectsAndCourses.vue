<script setup>
import weatherNow from '@/assets/images/projects/weather-now.png';
import spaceTourismWebsite from '@/assets/images/projects/space-tourism-website.png';
import rockPaperScissors from '@/assets/images/projects/rock-paper-scissors.png';
import countriesApp from '@/assets/images/projects/countries-app.png';
import weatherApp from '@/assets/images/projects/weather-app.png';

import WebProjectsWithVanillaJavaScript from '@/assets/images/courses/20-web-projects-with-vanilla-javascript.jpg';
import KevinPowell from '@/assets/images/courses/kevin-powell.jpg';
import ModernJavascriptFromTheBeginning from '@/assets/images/courses/modern-javascript-from-the-beginning.jpg';
import ReactFrontToBack from '@/assets/images/courses/react-front-to-back.jpg';
import ReactTheCompleteGuide2023 from '@/assets/images/courses/react-the-complete-guide-2023.jpg';
import TypeScriptCrashCourse from '@/assets/images/courses/typescript-crash-course.jpg';

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

const courses = [
  {
    id: 1,
    title: 'Modern JavaScript From The Beginning',
    author: 'Brad Traversy',
    description:
      'A 36-hour master course to take you from beginner to advanced JavaScript',
    technology: 'javascript',
    screenshot: ModernJavascriptFromTheBeginning,
    link: 'https://www.udemy.com/course/modern-javascript-from-the-beginning/',
  },
  {
    id: 2,
    title: 'React - The Complete Guide 2023 (incl. React Router & Redux)',
    author: 'Maximilian Schwarzmüller',
    description:
      'Dive in and learn React.js from scratch! Learn React, Hooks, Redux, React Router, Next.js, Best Practices and way more!',
    technology: 'react',
    screenshot: ReactTheCompleteGuide2023,
    link: 'https://www.udemy.com/course/react-the-complete-guide-incl-redux',
  },
  {
    id: 3,
    title: 'React Front To Back',
    author: 'Brad Traversy',
    description:
      'Learn modern React by building 4 projects including a Firebase 9 app and a full stack MERN app',
    technology: 'react',
    screenshot: ReactFrontToBack,
    link: 'https://www.udemy.com/course/react-front-to-back-2022/',
  },
  {
    id: 4,
    title: '20 Web Projects With Vanilla JavaScript',
    author: 'Brad Traversy',
    description:
      'Build 20 mini frontend projects from scratch with HTML5, CSS & JavaScript (No frameworks or libraries)',
    technology: 'javascript',
    screenshot: WebProjectsWithVanillaJavaScript,
    link: 'https://www.udemy.com/course/web-projects-with-vanilla-javascript/',
  },
  {
    id: 5,
    title: 'Front-end web development & design tips, tricks and tutorials',
    author: 'Kevin Powell',
    description: `The internet calls him the 'CSS Evangelist' for a reason. :D`,
    technology: 'css',
    screenshot: KevinPowell,
    link: 'https://www.youtube.com/channel/UCJZv4d5rbIKd4QHMPkcABCw',
  },
  {
    id: 6,
    title: 'TypeScriptCrashCourse',
    author: 'Brad Traversy',
    description:
      'The basics of TypeScript in this beginner-friendly crash course',
    technology: 'typescript',
    screenshot: TypeScriptCrashCourse,
    link: 'https://youtu.be/BCg4U1FzODs',
  },
];

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
  <div class="projects-and-courses">
    <h2>Projects 'n' Courses</h2>

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

    <div class="courses">
      <h4>Courses and tutorials I've completed to sharpen my skills.</h4>

      <div class="cards-wrapper">
        <div v-for="course in courses" :key="course.id" class="card">
          <img :src="course.screenshot" :alt="course.title" />
          <span :class="`technology ${course.technology}`"></span>

          <div class="card-body">
            <h5>
              {{ course.title }}
            </h5>

            <p>{{ course.description }}</p>
          </div>
        </div>
      </div>
    </div>

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
  </div>
</template>
