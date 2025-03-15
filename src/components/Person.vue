<script setup>
let person={
  name:"Sakib al hasan",
  age:"40",
  phone:"0185556677",
  address:"Cumilla"
}

</script>

<template>

    <p>Name:{{ person.name }}</p>
    <p>Age:{{ person.age }}</p>
    <p>Phone:{{ person.phone }}</p>
    <p>Address:{{ person.address }}</p>

</template>

<style scoped></style>