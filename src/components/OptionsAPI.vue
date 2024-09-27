<template>
    <div class="greetings">
        <h1>Options API</h1>
        <p>Number: {{ number }}</p>
        <p>String: {{ string }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            number:100,
            string:'Hello Options!'
        };
    },
    mounted() {
        console.log('Number: ', this.number);
        console.log('String: ',this.string );
    }
};
</script>

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