<template>
  <div class="project">
    <a
      target="_blank"
      rel="noopener noreferrer"
      href="https://ispyleipzig.netlify.app"
    >
      <h1>ispy</h1>
      <img class="image" src="../assets/mockups.png" alt="" />
    </a>
    <div class="info">
      <div class="row">
        <div class="detail">
          <h3>role</h3>
          <p>designer and developer</p>
        </div>
        <div class="detail">
          <h3>project type</h3>
          <p>web and mobile app</p>
        </div>
        <div class="detail">
          <h3>when</h3>
          <p>2021-2022</p>
        </div>
      </div>

      <div class="description row">
        <h3>description</h3>
        <p>
          ispy is an alternative to the current dating app model. it is more
          than a dating app, it is also a social networking tool that can
          connect two or more people who have met and want to meet again.
        </p>
        <p>
          this idea was born out of my own frustration with dating apps, and the
          very shallow model of swiping through photos and profiles until some
          feeling of connection is sparked. why not follow your instincts in
          real life? i wanted to create a tool for people to reconnect after
          those encounters.
        </p>
        <p>
          i started with figma wire framing and then used vue.js, html, css,
          firebase, and netlify to make the app come to life. it is still a work
          in progress and i plan to launch it in spring/summer '22.
        </p>
      </div>
    </div>
    <router-link to="devhaus"><h1 class="next">next project</h1></router-link>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
