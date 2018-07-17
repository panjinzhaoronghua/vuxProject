<template>
  <div>
    <group>
      <cell title="Total" value="￥1024"></cell>
      <cell-form-preview :list="list"></cell-form-preview>
    </group>
    <x-icon type="ios-arrow-up" size="30"></x-icon>
    <router-link to="/foo">Go to Foo</router-link>
  </div>
</template>
<script>
  import { Group, Cell, CellFormPreview, Icon } from 'vux'
  export default {
    components: {
      CellFormPreview,
      Group,
      Cell,
      Icon
    },
    data() {
      return {
        list: [{
          label: 'Apple',
          value: '3.29'
        }, {
          label: 'Banana',
          value: '1.04'
        }, {
          label: 'Fish',
          value: '8.00'
        }]
      }
    }
  }
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
