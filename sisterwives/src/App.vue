<template>
  <div id="app">
    <router-link class="home-link" to="/"
      ><h1>sisterwives studio</h1></router-link
    >
    <div class="page">
      <div class="view">
        <router-view></router-view>
      </div>
      <div class="logo">
        <img src="./assets/sisterwiveslogo.png" alt="" />
      </div>
    </div>
    <footer>
      <a
        target="_blank"
        rel="noopener noreferrer"
        href="https://www.instagram.com/sisterwives.studio/"
      >
        <span
          class="iconify"
          data-icon="ant-design:instagram-filled"
          style="color: black"
        ></span
      ></a>
      <a href="mailto:info@sisterwives.studio">info@sisterwives.studio</a>
    </footer>
  </div>
</template>

<style>
@font-face {
  font-family: "Metana";
  src: local("Metana"), url(./fonts/NeueMetana-Regular.otf) format("opentype");
}

body {
  background-image: url("./assets/sisterwivesbackground.png");
  background-size: fill;
  font-family: "Metana";
  overflow: hidden;
}

h1 {
  font-family: "Metana-bold";
  font-size: 60px;
  margin-left: 2rem;
}

.home-link {
  text-decoration: none;
  color: #e9e9e9;
  -webkit-text-stroke: 1px black;
}

.home-link:hover {
  color: rgb(223, 176, 21);
  font-style: italic;
}

.link {
  text-decoration: none;
  color: black;
}

.link:hover {
  font-style: italic;
  color: #e9e9e9;
  -webkit-text-stroke: 1px black;
}

.page {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.view {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.logo img {
  height: 70vh;
}

footer {
  display: flex;
  align-items: center;
  position: fixed;
  bottom: 0;
  margin: 2rem;
}

.iconify {
  font-size: 28px;
  margin-right: 2rem;
}

footer a {
  color: black;
  text-decoration: none;
}

@media only screen and (max-width: 750px) {
  h1 {
    font-size: 35px;
    margin-left: 0;
  }

  .page {
    flex-direction: column-reverse;
    align-items: flex-start;
  }

  .logo img {
    height: 275px;
  }

  footer {
    margin: 1rem;
  }
}
</style>
