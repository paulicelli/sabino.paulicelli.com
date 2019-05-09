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
          'p': 'Lead and Learn',
          'h5': '2018'
        },
        {
          'n': 2,
          'p': 'In-Store Guest Trainer',
          'h5': '2014'
        },
        {
          'n': 3,
          'p': 'Training Facilitator',
          'h5': '2011 - actual'
        },
        {
          'n': 4,
          'p': 'Market Core Facilitator',
          'h5': '2012'
        },
        {
          'n': 5,
          'p': 'User Acceptance Training',
          'h5': '2012'
        },
        {
          'n': 6,
          'p': 'User Acceptance Training',
          'h5': '2011'
        },
        {
          'n': 7,
          'p': 'Training Mentor',
          'h5': '2011'
        },
        {
          'n': 8,
          'p': 'Facilitation Skills',
          'h5': '2011'
        },
        {
          'n': 9,
          'p': 'IS&T Champion',
          'h5': '2010 - 2017'
        },
        {
          'n': 10,
          'p': ' CoreTraining Mentor',
          'h5': '2010'
        },
        {
          'n': 11,
          'p': 'Apple European Employee Forum Delegate',
          'h5': '2010'
        },
        {
          'n': 12,
          'p': 'Training Mentor',
          'h5': '2011'
        },
        {
          'n': 13,
          'p': 'Genius enrollment',
          'h5': '2009'
        },
      ],
      'work': [
        {
          'n': 1,
          'p': 'Tech Support'+'<br>'+'Data Port - Apple PR.',
          'h5': '2008'
        },
        {
          'n': 2,
          'p': 'Architecture designer'+'<br>'+'André Benaim',
          'h5': '2007'
        },
        {
          'n': 3,
          'p': 'Apple Macintosh Solution Consultant'+'<br>'+'InStore',
          'h5': '2007'
        },
        {
          'n': 4,
          'p': 'Apple Brand Specialist'+'<br>'+'InStore',
          'h5': '2006'
        },
        {
          'n': 5,
          'p': 'Community Service'+'<br>'+'AISM',
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
</style>
