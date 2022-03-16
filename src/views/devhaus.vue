<template>
  <div class="project">
    <a
      target="_blank"
      rel="noopener noreferrer"
      href="https://devhausleipzig.de"
    >
      <h1>devhaus</h1>
      <img class="image" src="../assets/devhaus.png" alt="" />
    </a>
    <div class="info">
      <div class="row">
        <div class="detail">
          <h3>role</h3>
          <p>designer and developer</p>
        </div>
        <div class="detail">
          <h3>project type</h3>
          <p>website</p>
        </div>
        <div class="detail">
          <h3>when</h3>
          <p>Dec 2020</p>
        </div>
      </div>
      <div class="description row">
        <h3>description</h3>
        <p>
          devhaus leipzig is an educational community dedicated to providing
          their members with instruction to become successful frontend
          developers. as an alumni of devhaus, i was honored to work on their
          webpage.
        </p>
        <p>
          we started by pulling ideas from inspirational companies providing
          similar services, creative agencies as well as educational
          institutions. we created wireframes and style guides in figma. once
          those were approved we began to develop the site using vue.js, html,
          css, and netlify.
        </p>
        <p>
          i was pleased to have the support of my former instructor Gabriel
          Heinrich while working on this project. he guided me through the
          process as it was my first freelance project after graduating from the
          coding bootcamp.
        </p>
      </div>
    </div>
    <router-link to="traumgaben"
      ><h1 class="next">next project</h1></router-link
    >
  </div>
</template>

<script>
export default {};
</script>
