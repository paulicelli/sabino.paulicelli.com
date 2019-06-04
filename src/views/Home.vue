<template>
  <div class="home">
    <main>
      <img id="foto" src="@/assets/sabi.jpg" alt="foto">
      <h1>developer</h1>
      <p>
        Hi! I'm a MacOS, iOS, and formerly windows, support advisor and technician, with more than <span style="text-decoration: underline;">20 years of experience on the field.</span> My career started suddenly when I left Architecture studies, which left me with a not negligible luggage of digital art experience. I actually work as <span style="text-decoration: underline;">Genius for Apple Retail,</span> at Oriocenter near Bergamo. I like my job and moreover I feel lucky for having the great opportunity to live everyday with those special persons my colleagues are. I like to see them grow up and feed their passions, I help whenever I can sharing my knowledge, coaching by example, smile and joke whenever is appropriate. I admire and prefer the kind of "mentor" over the "leader", the human over the alpha male, and the diversity (gender, race, religion) over the conformism.
      </p>
      <h3>experience</h3>
      <p>
        Natural born learner, I started in 2011 to study C and algorithms, which has become my only passion in 2014 with the disclosure of Swift. Since then, studying whenever and wherever possible, I had some opportunity to exercise with <span style="text-decoration: underline;">static websites (html, css, vanilla javascript),</span> <span style="text-decoration: underline;">Wordpress themes development,</span> an <span style="text-decoration: underline;">iOS app</span> for learning purposes (and a ton of Swift Playgrounds), and lately approaching <span style="text-decoration: underline;">Laravel</span> and <span style="text-decoration: underline;">VueJS.</span>
      </p>
      <h3>looking for</h3>
      <p>
        The work environment I dream about is physical or remote, showing noticeable diversity, human values, tight teamwork, friendship, open feedback, oriented toward new technologies.
      </p>
    </main>
  </div>
</template>

<script>
export default {
  name: 'home',
  components: {
    //
  }
}
</script>

<style scoped>
.home {
  width: 80vw;

  padding: 1em 1em 1em 2em;
}

#foto {
  width: 100%;
  border: solid var(--main-color) 1em;
}

h1 {
  text-transform: capitalize;
  padding: 1.5em 0;
}

h3 {
  text-transform: capitalize;
  padding: 1.5em 0;
}

main {
  margin: 5em 0;
}

@media (min-width: 48rem) {
  #foto {
    width: 16em;
    display: initial;
    float: left;
    margin: 0 2em 1em 0;
  }

  .home {
  width: 100vw;

  padding: 0;
}

  main {
    margin: 4em 10vw;
    width: 80vw;
  }
}
</style>
