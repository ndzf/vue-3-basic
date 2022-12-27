<script>

export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      const currentCounter = this.count;
      (currentCounter <= 0) ? this.count : this.count--;
    }
  }
};
</script>

<template>
  <h1>Hello World</h1>
</template>

<style>
.app-wrapper {
  display: flex;
  justify-content: center;
}

.container {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 1rem;
}

button.btn {
  background-color: #6777ef;
  font-size: 1rem;
  color: white;
  padding: .5rem;
}

p {
  margin: 0;
}
</style>
