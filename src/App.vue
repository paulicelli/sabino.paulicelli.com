<template>
  <div id="app">
    <header-title/>
    <nav>
      <li><router-link to="/"><i>home</i></router-link></li>
      <li><router-link to="/"><i>about</i></router-link></li>
      <li><router-link to="/"><i>works</i></router-link></li>
      <li><router-link to="/"><i>skills</i></router-link></li>
      <li><router-link to="/"><i>passions</i></router-link></li>
    </nav>
    <router-view/>
  </div>
</template>

<script>
import HeaderTitle from '@/components/HeaderTitle.vue'

export default {
  name: 'home',
  components: {
    HeaderTitle
  }
}
</script>


<style>
:root {
    /* COLORS */
    --main-color: Black;
    --accent-color: Red;

    --background: AntiqueWhite;

    --bg-color: rgb(230, 230, 230);

    /* FONTS */
    --header-font: "Futura", "Arial Black", sans-serif;
    --main-font: "Baskerville", "Times New Roman", serif;
    --main-font-size: 1rem;

    /* BREAKPOINTS */
    --phone-landscape: 30rem; /* 480px when font-size is 16px (iPhone landscape, phablets portrait maybe) */
    --tablet-portrait: 48rem; /* 768px when font-size is 16px (iPad portrait, phablets landscape maybe) */
    --tablet-landscape: 64rem; /* 1024px when font-size is 16px (iPad landscape and small desktops) */
    --desktop: 80rem; /* 1280px when font-size is 16px (fair desktop, should not change over this width) */

    /* SOME DIMENSIONS */
    --header-height: 4rem;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--main-font);
    color: var(--main-color);

    background-color: var(--background);
}

h1, h2, h3 {
    font-family: var(--header-font);
    font-weight: 300;
}

h1 {
    font-size: 2em;
    text-align: left;
}

h2 {
    font-size: 1.7em;
}

h3 {
    font-size: 1.3em;
}

p {
    font-size: 1.0em;
    font-weight: 300;
    line-height: 1.5em;
}

a {
    color: inherit;
    text-decoration: none;
}

a:hover {
    color: inherit;
    text-decoration:underline;
}

a:visited {
    color: inherit;
    text-decoration: none;
}

a:focus {
    color: inherit;
    text-decoration: none;
}

nav {
  box-sizing: content-box;
  background-color: AntiqueWhite; 

  position: fixed;
  right: 0;
  top: 50vh;
  width: calc(100vw - (80vw + 1em));
  margin: 1em 0;
  padding: 0 1em;

  border-left: solid var(--main-color) 1em;

  list-style: none;

  transition: right ease-out 1s;
}

nav > li {
  text-align: right;
  padding: 0.2em 0;
}

.nav-hidden {
  right: calc(-25vw - 1em);
}

</style>
