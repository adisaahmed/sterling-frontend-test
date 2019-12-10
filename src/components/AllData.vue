<template>
  <div>
    <div>
      <ul>
        <li v-bind:key="alldata.id" v-for="alldata in alldatas.results">
          {{alldata.name}}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    name: "AllData",
    props: ["alldatas"]
  }
</script>