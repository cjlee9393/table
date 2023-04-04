<template>
    <p>DataBTable</p>
    <div class="col-12">
        <b-table :items="items"
            :fields="['name', 'number', 'descA', 'descB', 'descC', 'descD', 'descE', 'descF', 'square', 'cube', 'quad', 'pent', 'sext']"
            hover
            striped>
        </b-table>
    </div>
</template>

<script>
export default {
  name: 'DataBTable',
  props: {
    items: {
        type: Array,
        default: () => [],
    }
  }
};
</script>