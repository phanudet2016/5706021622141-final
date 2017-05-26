<template>
<div class="hello">
  <table class="table">
  <thead>
    <tr>
      <th>#</th>
      <th>ชื่อวิชา</th>
      <th>หน่วยกิต</th>
      <th>เกรด</th>
      <th>Delete</th>
    </tr>
  </thead>
  </table>
  <!-- <v-for="list in menu"> -->
    <list v-for="list in menu" :list="list" :remove="remove" :index="$index"></list>
  </div>
</div>
</template>

<script>
import List from './List'
export default {
  props: ['menu', 'remove'],
  data () {
    return {}
  },
  components: {
    List
  }
}
</script>

<style scoped>
h1 {
  color: #42b983;
}
</style>
