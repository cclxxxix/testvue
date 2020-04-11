<template>
  <div>
    <b-table striped hover :items="teachers">
         <template v-slot:cell(name)="data">
        <router-link :to="`/teachers/${data.value}`">{{ data.value }}</router-link>
      </template>
    </b-table>
  </div>
</template>

<script>
import teachers from '../data/Teachers.js'
  export default {
    data() {
      return {
        teachers
      }
    }
  }
</script>