<script setup>
import { ref } from "vue";
import Person from "./components/Person.vue";
import CounterApp from "./components/CounterApp.vue";
import Student from "./components/Student.vue";

let headline = ref("IsDB-BISEW");
let toggle = ref(true);
let paragraph_id = ref("asset");

const changeId=()=>{
  paragraph_id.value="paragraph"
}

</script>

<template>
  <div>
    <h1 v-if="toggle" v-html="headline"></h1>

    <p :id="paragraph_id">
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Consequuntur
      sequi architecto, repellat tempora, dolorum recusandae, aliquam
      necessitatibus enim unde distinctio ut adipisci optio provident earum
      perferendis sed suscipit omnis saepe!
    </p>
    <br />

    <input type="text" v-model="headline" placeholder="headline" /><br><br>

    <button @click="toggle = !toggle">Show/Hide</button>
    <button @click="changeId">Change ID</button>

    <Person /><br />
    <CounterApp /><br />
    <Student />
  </div>
</template>

<style scoped></style>
