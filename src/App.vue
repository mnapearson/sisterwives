<template>
  <div class="pagewrapper" id="app">
    <div class="">
      <router-link class="home-link" to="/">sisterwives studio</router-link>
    </div>
    <div class="nav">
      <router-link class="link" to="/portfolio">
        <h1>portfolio</h1></router-link
      >

      <router-link class="link" to="/shop"> <h1>shop</h1></router-link>

      <!-- <router-link class="link" to="/radio"><h1>radio</h1></router-link> -->

      <router-link class="link" to="/contact"> <h1>contact</h1></router-link>
    </div>

    <div class="page">
      <router-view></router-view>
    </div>
    <footer>
      <div class="logo">
        <router-link to="/">
          <img src="./assets/sisterwiveslogo.png" alt=""
        /></router-link>
      </div>
      <a href="mailto:info@sisterwives.studio"
        ><p>info@sisterwives.studio</p></a
      >
    </footer>
  </div>
</template>

<style>
@font-face {
  font-family: "Metana";
  src: local("Metana"), url(./fonts/NeueMetana-Regular.otf) format("opentype");
}

*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  margin: 1rem;
  overscroll-behavior: none;
  background-color: #e9e9e9;
  font-family: "Metana";
}

.pagewrapper {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.home-link {
  font-family: "Metana-bold";
  text-decoration: none;
  color: #b9a918;
  -webkit-text-stroke: 1px black;
  font-size: 44px;
  width: 350px;
  line-height: 2.5rem;
}

.home-link:hover {
  color: #e9e9e9;
  font-style: italic;
}

.nav {
  display: flex;
  margin-bottom: 3rem;
}

h1,
a {
  text-decoration: none;
  color: black;
  font-family: "Metana-bold";
  font-size: 16px;
  margin-right: 0.5rem;
  text-align: center;
}

h1:hover {
  font-style: italic;
  color: #e9e9e9;
  -webkit-text-stroke: 1px black;
}

h2 {
  font-size: 16px;
}

h3 {
  font-size: 14px;
  text-transform: uppercase;
  text-decoration: underline;
}

p {
  font-size: 12px;
  margin: 1rem;
}

.page {
  display: flex;
  flex-grow: 1;
  flex-direction: column;
  justify-content: center;
  align-items: center;
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

.logo img {
  width: 375px;
}

footer {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 3rem;
}

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

.info {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-start;
  line-height: 1.5rem;
}

.row {
  max-width: 50%;
  margin: 1rem;
}

.detail {
  display: flex;
  flex-direction: column;
}

.detail p {
  margin: 0;
}

.next {
  margin-top: 2rem;
}

@media only screen and (max-width: 700px) {
  .info {
    flex-direction: column;
    align-items: center;
  }

  .row {
    max-width: 80%;
  }

  .detail {
    text-align: center;
  }
}
</style>
