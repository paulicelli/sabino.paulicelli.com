<template>
  <div id="app">
    <header-title v-on:hide-nav="hideNav"/>
    <nav :class="{ 'nav-hidden': isNavHidden }">
      <li v-on:click="waitAndHideNav"><router-link to="/"><i>home</i></router-link></li>
      <li v-on:click="waitAndHideNav"><router-link to="/about"><i>about</i></router-link></li>
      <li v-on:click="waitAndHideNav"><router-link to="/resume"><i>resume</i></router-link></li>
      <li v-on:click="waitAndHideNav"><router-link to="/works"><i>works</i></router-link></li>
      <li v-on:click="waitAndHideNav"><a href="./201906_cv_sabino_paulicelli.pdf"><i>download PDF</i></a></li>
    </nav>
    <router-view/>
  </div>
</template>

<script>
import HeaderTitle from '@/components/HeaderTitle.vue'

export default {
  components: {
    HeaderTitle
  },
  data() {
    return {
      'isNavHidden': true,
      'navTimer': null
    }
  },
  methods: {
    waitAndHideNav() {
      if (this.navTimer != null){
        clearTimeout(this.navTimer);
      }
      this.navTimer = setTimeout(this.hideNav, 2000);
      this.scrollTop()
    },
    hideNav() {
      this.isNavHidden = !this.isNavHidden
    },
    scrollTop() {
      document.body.scrollTop = document.documentElement.scrollTop = 0;
    }
  }
}
</script>


<style>
:root {
    /* COLORS */
    --main-color: rgba(12, 12, 10, 0.8);
    --accent-color: #f9423a;

    --background: #f6f3ea;

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

h1, h2, h3, h4, h5, h6 {
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
    color: var(--accent-color);
    text-decoration: none;
}

a:hover {
    color: var(--accent-color);
    text-decoration:underline;
}

a:visited {
    color: var(--accent-color);
    text-decoration: none;
}

a:focus {
    color: var(--accent-color);
    text-decoration: none;
}

nav {
  box-sizing: content-box;
  background-color: var(--background); 

  position: fixed;
  right: 0;
  top: 50vh;
  width: calc(100vw - (80vw + 1em));
  margin: 1em 0;
  padding: 0 1em;

  border-left: solid var(--main-color) 1em;

  list-style: none;

  transition: right ease-out 0.5s;
}

nav > li {
  font-size: 1.1em;
  text-transform: capitalize;
  text-align: right;
  padding: 0.2em 0;
}

.nav-hidden {
  right: calc(-25vw - 1em);
}

.router-link-exact-active {
  font-weight: bold;
}

@media (min-width: 48rem) {
  nav {
    box-sizing: content-box;
    background-color: var(--background); 

    position: initial;
    width: 80vw;
    margin: 2em 10vw 0 10vw;
    padding: 0.5em 0;

    border-top: solid var(--main-color) 4px;
    border-bottom: solid var(--main-color) 4px;
    border-left: none;

    list-style: none;
    transition: none;

    display: flex;
    justify-content: space-around;
  }
}
</style>
