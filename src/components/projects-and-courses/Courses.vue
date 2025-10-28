<script setup>
import WebProjectsWithVanillaJavaScript from '@/assets/images/courses/20-web-projects-with-vanilla-javascript.jpg';
import KevinPowell from '@/assets/images/courses/kevin-powell.jpg';
import ModernJavascriptFromTheBeginning from '@/assets/images/courses/modern-javascript-from-the-beginning.jpg';
import ReactFrontToBack from '@/assets/images/courses/react-front-to-back.jpg';
import ReactTheCompleteGuide2023 from '@/assets/images/courses/react-the-complete-guide-2023.jpg';
import TypeScriptCrashCourse from '@/assets/images/courses/typescript-crash-course.jpg';

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
</script>

<template>
  <div class="courses">
    <h4>Courses and tutorials I've completed to sharpen my skills.</h4>

    <div class="cards-wrapper">
      <div v-for="course in courses" :key="course.id" class="card wide">
        <div class="image-wrapper">
          <img :src="course.screenshot" :alt="course.title" />
          <span :class="`technology ${course.technology}`"></span>
        </div>

        <div class="card-body">
          <h5>
            {{ course.title }}
          </h5>

          <p>{{ course.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
