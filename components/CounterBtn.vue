<template>
  <div class="counter">
    <button @click="increament">+</button>
    <p>{{ count }}</p>
    <button @click="decreament">-</button>
  </div>
</template>

<script setup>
// composition api====================

// for using com api add attribute in script tag

const count = ref(0);

function increament() {
  count.value++;
}

function decreament() {
  count.value--;
  console.log(count);
}

// /option api

// export default {
//   data() {
//     return {
//       count: 0,
//     };
//   },

//   methods: {
//     increament() {
//       this.count++;
//     },
//     decreament() {
//       this.count--;
//     },
//   },
// };
</script>

<style lang="scss" scoped>
.counter {
  display: flex;
  gap: 1rem;
  align-items: center;
  p {
    font-size: 1rem;
    color: red;
    padding: 1rem;
    font-weight: bold;
  }

  button {
    border: 1px solid #333;
    padding: 0.5rem 1rem;
    background: black;
    color: #fff;
    font-size: 1rem;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.45s ease-in;
    &:hover {
      background: rgba(0, 0, 0, 0.8);
    }
  }
}
</style>
