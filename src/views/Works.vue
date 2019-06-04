<template>
  <div class="works">
    <main>
      <h1>works</h1>
      <p>
        Of course in my learning journey I wrote a ton of code, sometimes for me or supporting other people's work. However, even if only as second job, my passion led me to at least 3 finished jobs I did and I'm glad to show in this resume.
      </p>
      <h3>zelandia travel (work in progress)</h3>
      <p>
        A website for a Tour Agency, written in VueJS as a PWA. The backend for data and the admin page in Laravel and a faster API served by a Vapor/Swift server.
      </p>
      <h3>this resume as website</h3>
      <p>
        Willing to show some skills for an interview, I did this website in 2 half-days, very quick and dirty :] , using VueJS. The source code is on Github at <a href="https://github.com/paulicelli/sabino.paulicelli.com">https://github.com/paulicelli/sabino.paulicelli.com</a>.
      </p>
      <h3>surflanguage.com</h3>
      <p>
        A website for a Lingustic / Surf School, coded in PHP, multilanguage strings served by an SQLite database.
      </p>
      <h3>MESC: Mindfulness Experience Sampling for Children</h3>
      <p>
        An iPad app made for a psichologic study on children. Made in Xcode and Swift.
      </p>
      <h3>panfrutta.it</h3>
      <p>
        My very first finished website, made for a friend using Bootstrap.
      </p>
      <h3>( work in progress )</h3>
      <p>
        A website for a Tour Agency, written in VueJS as a PWA. 2 backends for data, the admin page in Laravel and an API served by a Vapor/Swift server.
      </p>
      <h3>links</h3>
      <table-list :content="works" />
    </main>
  </div>
</template>

<script>
import TableList from '@/components/TableList.vue'

export default {
  name: 'works',
    components: {
      TableList
  },
  data() {
    return {
      'works': [
        {
          'n': 1,
          'p': '<a href="https://www.zelandiatravel.it">zelandiatravel.it</a>'+'<br>'+'Zelandia Travel di So.Im.Tour',
          'h5': '2019'
        },
        {
          'n': 2,
          'p': '<a href="https://sabino.paulicelli.com">this website</a>'+'<br>'+'sabino.paulicelli.com',
          'h5': '2019'
        },
        {
          'n': 3,
          'p': '<a href="https://www.surflanguage.com">surflanguage.com</a>'+'<br>'+'Surf Language Ass. Culturale',
          'h5': '2018'
        },
        {
          'n': 4,
          'p': '<a href="https://www.panfrutta.it">panfrutta.it</a>'+'<br>'+'Non solo frutta Snc',
          'h5': '2017'
        }
      ]
    }
  }
}
</script>

<style scoped>
.works {
  width: 80vw;
  padding: 2em 1em 1em 2em;
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
  margin: 2em 0;
}

@media (min-width: 48rem) {
  .works {
  width: 100vw;

  padding: 0;
}

  main {
    margin: 4em 10vw;
    width: 80vw;
  }
}
</style>
