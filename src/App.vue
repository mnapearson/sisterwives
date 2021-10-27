<template>
  <div id="app">
    <router-link class="home-link" to="/"
      ><h1>sisterwives studio</h1></router-link
    >
    <div class="nav">
      <router-link class="link" to="/portfolio">
        <h1>portfolio</h1></router-link
      >

      <router-link class="link" to="/shop"> <h1>shop</h1></router-link>

      <router-link class="link" to="/contact"> <h1>contact</h1></router-link>
    </div>
    <div class="page">
      <div class="view">
        <router-view></router-view>
      </div>
      <div class="logo">
        <router-link to="/">
          <img src="./assets/sisterwiveslogo.png" alt=""
        /></router-link>
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
  background-color: #e9e9e9;
  font-family: "Metana";
}

h1 {
  font-family: "Metana-bold";
  font-size: 30px;
  margin-left: 2rem;
}

.home-link {
  text-decoration: none;
  color: #b9a918;
  -webkit-text-stroke: 1px black;
}

.home-link h1 {
  font-size: 50px;
}

.home-link:hover {
  color: #e9e9e9;
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

.nav {
  display: flex;
  align-items: flex-start;
  margin-top: -2.5rem;
}

.nav h1 {
  font-size: 20px;
}

.page {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100%;
  -webkit-animation: fade-in 1.75s cubic-bezier(0.39, 0.575, 0.565, 1) both;
  animation: fade-in 1.75s cubic-bezier(0.39, 0.575, 0.565, 1) both;
}

@-webkit-keyframes fade-in {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@keyframes fade-in {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

.view {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
}

.logo img {
  height: 70vh;
}

.logo:hover {
  -webkit-animation: heartbeat 1.75s ease-in-out infinite both;
  animation: heartbeat 1.75s ease-in-out infinite both;
}

@-webkit-keyframes heartbeat {
  from {
    -webkit-transform: scale(1);
    transform: scale(1);
    -webkit-transform-origin: center center;
    transform-origin: center center;
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
  10% {
    -webkit-transform: scale(0.91);
    transform: scale(0.91);
    -webkit-animation-timing-function: ease-in;
    animation-timing-function: ease-in;
  }
  17% {
    -webkit-transform: scale(0.98);
    transform: scale(0.98);
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
  33% {
    -webkit-transform: scale(0.87);
    transform: scale(0.87);
    -webkit-animation-timing-function: ease-in;
    animation-timing-function: ease-in;
  }
  45% {
    -webkit-transform: scale(1);
    transform: scale(1);
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
}
@keyframes heartbeat {
  from {
    -webkit-transform: scale(1);
    transform: scale(1);
    -webkit-transform-origin: center center;
    transform-origin: center center;
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
  10% {
    -webkit-transform: scale(0.91);
    transform: scale(0.91);
    -webkit-animation-timing-function: ease-in;
    animation-timing-function: ease-in;
  }
  17% {
    -webkit-transform: scale(0.98);
    transform: scale(0.98);
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
  33% {
    -webkit-transform: scale(0.87);
    transform: scale(0.87);
    -webkit-animation-timing-function: ease-in;
    animation-timing-function: ease-in;
  }
  45% {
    -webkit-transform: scale(1);
    transform: scale(1);
    -webkit-animation-timing-function: ease-out;
    animation-timing-function: ease-out;
  }
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
  p {
    font-size: 16px;
  }

  .home-link h1 {
    font-size: 28px;
    margin-bottom: 1rem;
    margin-top: 0;
  }

  .home-link {
    display: flex;
    justify-content: center;
  }

  h1 {
    font-size: 20px;
    margin-left: 0;
  }

  .nav {
    display: flex;
    justify-content: center;
  }

  .nav h1 {
    margin-left: 0;
    margin-right: 1rem;
  }

  .page {
    flex-direction: column-reverse;
    align-items: center;
    justify-content: center;
    margin-bottom: 4rem;
    text-align: center;
  }

  .logo {
    margin-top: 4rem;
    margin-bottom: 4rem;
  }

  .logo img {
    height: 275px;
  }

  footer {
    margin: 1rem;
    position: relative;
    justify-content: center;
  }
}
</style>
