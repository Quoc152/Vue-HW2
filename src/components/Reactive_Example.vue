<script setup>
    import { reactive, onMounted } from 'vue';  

    const state = reactive ({
        number: 100,
        string: 'Hello World!'
    });

    onMounted (() => {
        console.log('Number: ', state.number);
        console.log('String: ', state.string);
    });
</script>

<template>
    <div class="greetings">
        <h1>Reactive Example</h1>
        <p>Number: {{ state.number }}</p>
        <p>String: {{ state.string }}</p>
    </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
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