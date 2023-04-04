<!-- <script>
const headers = [
  {
    text: 'name',
    value: 'name'
  },
  {
    text: 'number',
    value: 'number'
  },
  {
    text: 'descA',
    value: 'descA'
  },
  {
    text: 'descB',
    value: 'descB'
  },
  {
    text: 'descC',
    value: 'descC'
  },
  {
    text: 'descD',
    value: 'descD'
  },
  {
    text: 'descE',
    value: 'descE'
  },
  {
    text: 'descF',
    value: 'descF'
  },
  {
    text: 'square',
    value: 'square'
  },
  {
    text: 'cube',
    value: 'cube'
  },
  {
    text: 'quad',
    value: 'quad'
  },
  {
    text: 'pent',
    value: 'pent'
  },
  {
    text: 'sext',
    value: 'sext'
  },
];

let myRows = 10000;
let items = new Array(myRows).fill('').map((v, index) => ({
  name: `name ${index}`,
  number: index,
  descA: `descA ${index}`,
  descB: `descB ${index}`,
  descC: `descC ${index}`,
  descD: `descD ${index}`,
  descE: `descE ${index}`,
  descF: `descF ${index}`,
  square: index * 2,
  cube: index * 3,
  quad: index * 4,
  pent: index * 5,
  sext: index * 6,
}));

import DataTable from './components/DataTable.vue';
import DataBTable from './components/DataBTable.vue';

export default {
  name: 'App',
  components: {
    // DataTable, // 사용할 컴포넌트로 등록
    DataBTable
  },
  data() {
    return {
      headers: headers,
      items: items
    };
  },
};
</script>-->

<!--
<template>
  <div id="app">
    <DataTable
      :headers="headers"
      :items="items"
    />
    <DataBTable 
      :items="items"
    />
  </div>
</template> -->

<template>
  <p> Hello </p>
  <div>
      <b-table striped hover :items="items"></b-table>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
      return {
          items: [
          { age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
          { age: 21, first_name: 'Larsen', last_name: 'Shaw' },
          { age: 89, first_name: 'Geneva', last_name: 'Wilson' },
          { age: 38, first_name: 'Jami', last_name: 'Carney' }
          ]
      }
  }
}
</script>