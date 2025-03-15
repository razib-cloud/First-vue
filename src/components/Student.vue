

<script lang="ts" setup>
let students =
`
<li>Kabir</li>
<li>RukRuk</li>
<li>Ranbir</li>
<li>Janjeer</li>
`

</script >



<template>
  <div>
    <h1>Student List</h1>
    <ul v-html="students"></ul>
    
  </div>
</template>

<style scoped>

</style>