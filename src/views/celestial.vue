<template>
  <div class="project">
    <a
      target="_blank"
      rel="noopener noreferrer"
      href="https://celestial-weather.netlify.app"
    >
      <h1>celestial weather</h1>
      <img class="image" src="../assets/celestial.png" alt="" />
    </a>
    <div class="ispy">
      <div class="col-left">
        <h3>role</h3>
        <p>designer and developer</p>
        <h3>project type</h3>
        <p>web app</p>
        <h3>when</h3>
        <p>August 2020</p>
      </div>
      <div class="col-right">
        <h3>description</h3>
        <p>
          celestial weather was the first project that i designed and developed
          during my coding bootcamp. i was inspired by the subject of REST API
          calls, and decided to incorporate a few interesting ones into my web
          app.
        </p>
        <p>
          the 3d cube was an experiment that i had a lot of fun with, this
          exploration in animation and design still intrigues me today and is
          something i hope to learn more about in the near future.
        </p>
        <p>
          i built this project with pure vanilla javascript, html5, and css. i
          used heroku to create my magic 8 ball api, and netlify to deploy the
          app.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.project {
  width: 100vw;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.image {
  max-width: 350px;
}

.ispy {
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
  margin-top: 2rem;
}

@media only screen and (max-width: 600px) {
  .ispy {
    flex-direction: column;
  }

  .col-left {
    width: 100%;
  }
}
</style>
