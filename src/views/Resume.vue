<template>
  <div class="resume">
    <main>
      <h1>resume</h1>
      <h3>in Apple</h3>
      <table-list :content="apple" />
      <h3>Work</h3>
      <table-list :content="work" />
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
      'apple': [
        {
          'n': 1,
          'p': 'Lead and Learn'+'<br>'+'Internal training organization and scheduling',
          'h5': '2018'
        },
        {
          'n': 2,
          'p': 'In-Store Guest Trainer'+'<br>'+'Internal training organization and scheduling',
          'h5': '2014'
        },
        {
          'n': 3,
          'p': 'Market Core Facilitator'+'<br>'+'Internal training for new employees',
          'h5': '2012'
        },
        {
          'n': 4,
          'p': 'User Acceptance Testing'+'<br>'+'Testing, bug hunt and report, feedback on internal software',
          'h5': '2012'
        },
        {
          'n': 5,
          'p': 'User Acceptance Testing'+'<br>'+'Testing, bug hunt and report, feedback on internal software',
          'h5': '2011'
        },
        {
          'n': 6,
          'p': 'Training Facilitator',
          'h5': '2011 - actual'
        },
        {
          'n': 7,
          'p': 'Facilitation skills'+'<br>'+'Training on more advanced internal training',
          'h5': '2011'
        },
        {
          'n': 8,
          'p': 'IS&T Champion'+'<br>'+'Hardware and software support for internal use technology and trainer',
          'h5': '2010 - 2017'
        },
        {
          'n': 9,
          'p': 'Training Mentor'+'<br>'+'Supporting new Store opening in Bergamo, Oriocenter Apple Store',
          'h5': '2010'
        },
        {
          'n': 10,
          'p': 'Apple European Employee Forum Delegate for North Italy Market',
          'h5': '2010'
        },
        {
          'n': 11,
          'p': 'Training Mentor'+'<br>'+'Assisting internal trainings',
          'h5': '2010'
        },
        {
          'n': 12,
          'p': 'Enrolled as Genius'+'<br>'+'Training experience in London and Rome, new Store opening in Milan, Carosello Apple Store',
          'h5': '2009'
        }
      ],
      'work': [
        {
          'n': 1,
          'p': 'Data Port (Apple Premium Reseller)'+'<br>'+'Tech Support and Advisor',
          'h5': '2008'
        },
        {
          'n': 2,
          'p': 'André Benaim Studio'+'<br>'+'Architecture designer',
          'h5': '2007'
        },
        {
          'n': 3,
          'p': 'InStore Srl'+'<br>'+'Apple Macintosh Solution Consultant',
          'h5': '2007'
        },
        {
          'n': 4,
          'p': 'InStore Srl'+'<br>'+'Apple Brand Specialist',
          'h5': '2006'
        },
        {
          'n': 5,
          'p': 'AISM'+'<br>'+'Community Service',
          'h5': '2003 - 2004'
        },
      ]
    }
  }
}
</script>

<style scoped>
.resume {
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
  .resume {
  width: 100vw;

  padding: 0;
}

  main {
    margin: 4em 10vw;
    width: 80vw;
  }
}
</style>
