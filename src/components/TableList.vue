<template>
  <div class="TableList">
      <table v-for='row in info' :key='info.n'>
        <tr>
          <td style="width: 66%; text-align: right; padding-right: 0.5em;"><p v-html="row.p"></p></td>
          <td style="width: 34p%; text-align: left;"><h5 v-html="row.h5"></h5></td>
        </tr>
      </table>
  </div>
</template>

<script>
export default {
  name: 'TableList',
  props: {
    content: Array
  },
  data() {
    return {
      info: this.content
    }
  }
}
</script>

<style scoped>
  h5 {
    text-transform: uppercase;
  }

  table {
    width: 100%;
    border-spacing: 0;
  }

  td {
    border-bottom: 1px solid var(--main-color);
    padding: 0.5em 0;
  }
</style>
