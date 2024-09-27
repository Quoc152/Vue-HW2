<script setup>
import { ref, onMounted } from 'vue';

const NumberRef = ref(100);
const StringRef = ref('Hello');

onMounted (() => {
  console.log('Number: ', NumberRef.value);
  console.log('String: ', StringRef.value);
});

</script>

<template>
  <div class="greetings">
    <h1>Ref Example</h1>
    <p>Number: {{ NumberRef }}</p>
    <p>String: {{ StringRef }}</p>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

p {
  font-size: 30px;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
