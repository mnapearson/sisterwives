<template>
  <div>
    <div class="portfolio">
      <h3>recent projects</h3>
      <div class="sites">
        <router-link to="ispy"> <h1 class="link">i spy</h1></router-link>

        <router-link to="devhaus"> <h1 class="link">devhaus</h1></router-link>
        <router-link to="traumgaben">
          <h1 class="link">traumgaben</h1></router-link
        >
        <router-link to="hendershot">
          <h1 class="link">hendershot</h1></router-link
        >
        <router-link to="celestial">
          <h1 class="link">celestial</h1></router-link
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Portfolio",
};
</script>

<style scoped>
h3 {
  margin-bottom: 2rem;
}

.link {
  margin-top: 0.5rem;
}

.portfolio {
  text-align: center;
}
</style>
