<template>
  <div class="project">
    <a
      target="_blank"
      rel="noopener noreferrer"
      href="https://wellroundedhoodlum.com"
    >
      <h1>hendershot</h1>
      <img class="image" src="../assets/hendershot.png" alt="" />
    </a>
    <div class="ispy">
      <div class="col-left">
        <h3>role</h3>
        <p>designer and developer</p>
        <h3>project type</h3>
        <p>website</p>
        <h3>when</h3>
        <p>July 2021</p>
      </div>
      <div class="col-right">
        <h3>description</h3>
        <p>
          Matthew Hendershot is a musician, podcast creator, producer, and well
          rounded hoodlum based in Leipzig, de. he required a landing page that
          could communicate his background and current projects, and provide a
          contact form for people to easily reach out to Matthew.
        </p>
        <p>
          i used inspiration from the logo he had provided me with, as well as
          the black and white photograph, to create the design for the landing
          page.
        </p>
        <p>
          due to the simplicity of this one page project, i used pure vanilla
          javascript, html5 and css to build the page.
        </p>
      </div>
    </div>
    <router-link to="celestial"><h1 class="next">next project</h1></router-link>
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
