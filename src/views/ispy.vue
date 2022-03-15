<template>
  <div class="project">
    <a
      target="_blank"
      rel="noopener noreferrer"
      href="https://ispyleipzig.netlify.app"
    >
      <h1>ispy</h1></a
    >
    <div class="images">
      <img class="mobile" src="../assets/ispymobile.png" alt="" />
      <img class="desktop" src="../assets/ispymockup.png" alt="" />
    </div>

    <div class="ispy">
      <div class="col-left">
        <h3>role</h3>
        <p>designer and developer</p>
        <h3>project type</h3>
        <p>web and mobile app</p>
        <h3>year</h3>
        <p>2021-2022</p>
      </div>
      <div class="col-right">
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
    <router-link to="portfolio"><h1 class="next">next project</h1></router-link>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
h2 {
  font-size: 16px;
}

h3 {
  font-size: 14px;
  text-transform: uppercase;
}

p {
  font-size: 12px;
}

.project {
  width: 100vw;
}

.images {
  display: flex;
  align-items: center;
  justify-content: center;
}

.mobile {
  max-height: 200px;
  padding: 1rem;
}

.desktop {
  max-width: 375px;
  padding: 1rem;
}

.ispy {
  text-align: left;
  display: flex;
  align-items: flex-start;
  line-height: 1.5rem;
}

.col-left {
  width: 50%;
  padding: 1rem;
}

.col-right {
  padding: 1rem;
}

.next {
  margin-top: 4rem;
}

@media only screen and (max-width: 600px) {
  .project {
    margin-top: 30rem;
  }

  .images {
    flex-direction: column;
  }

  .ispy {
    flex-direction: column;
  }

  .col-left {
    width: 100%;
  }
}
</style>
