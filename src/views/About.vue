<template>
  <div class="about">
    <main>
      <h1>about</h1>
      <table-list :content="personal" />
      <h3>studies</h3>
      <table-list :content="learning" />
      <h3>foreign<br>experiences</h3>
      <table-list :content="experiences" />
      <h3>passions</h3>
      <table-list :content="passions" />
    </main>
  </div>
</template>

<script>
import TableList from '@/components/TableList.vue'

export default {
  name: 'about',
  components: {
    TableList
  },
  data() {
    return {
      'personal': [
        {
          'n': 1,
          'p': '13th March, 1980',
          'h5': '<i class="fas fa-birthday-cake"></i>'
        },
        {
          'n': 2,
          'p': 'Calusco d\'Adda',
          'h5': '<i class="fas fa-city"></i>'
        },
        {
          'n': 3,
          'p': 'via san Giuliano, 84'+'<br>'+'24033 (BG) IT',
          'h5': '<i class="fas fa-map-marker-alt"></i>'
        },
        {
          'n': 4,
          'p': '<a href="tel:+393926801771>+39 392 680 1771</a>',
          'h5': '<i class="fas fa-phone"></i>'
        },
        {
          'n': 5,
          'p': '<a href="mailto:sabino@paulicelli.com">sabino@paulicelli.com</a>',
          'h5': '<i class="fas fa-envelope"></i>'
        },
        {
          'n': 6,
          'p': '<a href="https://twitter.com/SabinoP_">SabinoP_</a>',
          'h5': '<i class="fab fa-twitter"></i>'
        },
        {
          'n': 7,
          'p': '<a href="https://github.com/paulicelli">paulicelli</a>',
          'h5': '<i class="fab fa-github"></i>'
        },
        {
          'n': 8,
          'p': '<a href="https://stackoverflow.com/users/4242891/sabi">sabi</a>',
          'h5': '<i class="fab fa-stack-overflow"></i>'
        },
        {
          'n': 9,
          'p': '<a href="https://www.linkedin.com/in/sabino-paulicelli-3a1573120">Sabino Paulicelli</a>',
          'h5': '<i class="fab fa-linkedin"></i>'
        }
      ],
      'learning': [
        {
          'n': 1,
          'p': 'High School,'+'<br>'+'Liceo Scientifico',
          'h5': 'studies'
        },
        {
          'n': 2,
          'p': 'cat B/B1',
          'h5': 'driving l.'
        },
        {
          'n': 3,
          'p': 'swimming'+'<br>'+'martial arts',
          'h5': 'sports'
        },
        {
          'n': 4,
          'p': 'Architecture'+'<br>'+'Firenze University',
          'h5': 'studies'+'<br>'+'(discont.)'
        },
        {
          'n': 5,
          'p': 'Italian (native)'+'<br>'+'English (fluent)',
          'h5': 'languages'
        }
      ],
      'experiences': [
        {
          'n': 1,
          'p': 'English Course'+'<br>'+'Bashee\'s College',
          'h5': 'London (1995)'
        },
        {
          'n': 2,
          'p': 'Genius Training'+'<br>'+'Apple Store Regent St',
          'h5': 'London (2009)'
        },
        {
          'n': 3,
          'p': 'Apple European Employee Forum',
          'h5': 'London (2010)'
        },
        {
          'n': 4,
          'p': 'User Acceptance Testing',
          'h5': 'Cupertino (2011)'
        },
        {
          'n': 5,
          'p': 'User Acceptance Testing',
          'h5': 'Cupertino (2012)'
        },
        {
          'n': 6,
          'p': 'Apple European Education Summit',
          'h5': 'London (2018)'
        },
      ],
      'passions': [
        {
          'n': 1,
          'p': 'Board Games',
          'h5': '<i class="fas fa-heart"></i>'
        },
        {
          'n': 2,
          'p': 'Learning',
          'h5': '<i class="fas fa-heart"></i>'
        },
        {
          'n': 3,
          'p': 'Manual crafts',
          'h5': '<i class="fas fa-heart"></i>'
        },
        {
          'n': 4,
          'p': 'Walking with my wife',
          'h5': '<i class="fas fa-heart"></i>'
        },
        {
          'n': 5,
          'p': 'Old computer games',
          'h5': '<i class="fas fa-heart"></i>'
        },
        {
          'n': 5,
          'p': 'Stranger Things',
          'h5': '<i class="fas fa-heart"></i>'
        }
      ],
    }
  }
}
</script>

<style scoped>
.about {
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
</style>
