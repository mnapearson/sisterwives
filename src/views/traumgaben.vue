<template>
  <div class="project">
    <a
      target="_blank"
      rel="noopener noreferrer"
      href="http://henrikbaumgarten.de/"
    >
      <h1>traumgaben</h1>
      <img class="image" src="../assets/henrik.png" alt="" />
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
          <p>May 2021</p>
        </div>
      </div>
      <div class="description row">
        <h3>description</h3>
        <p>
          henrik baumgarten is a musician, composer and instructor based in
          leipzig, de. he needed to create an online prescense that could
          highlight the multiple projects that he is involved with. he also
          wished for a way for people who are interested in his work to easily
          contact him.
        </p>
        <p>
          i used figma to create the wireframes and layout for the intial
          design. my inspiration came from the beautiful photos that he had
          captured at his studio. they led me to create a clean and unique
          website for henrik.
        </p>
        <p>
          i built the website using vue.js, html5, css, email.js, and netlify.
        </p>
      </div>
    </div>
    <router-link to="hendershot"
      ><h1 class="next">next project</h1></router-link
    >
  </div>
</template>

<script>
export default {};
</script>
