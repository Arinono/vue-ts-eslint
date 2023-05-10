<template>
  <div class="container">
    old
    <button @click="up">
      count is {{ counter }}
    </button>
  </div>
</template>

<script>
export default {
  name: 'OldComponent',
  data: () => ({
    counter: 0,
  }),
  methods: {
    up() {
      this.counter++;
    },
  },
};
</script>

<style scoped>
.container {
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  align-items: center;
}

.container button {
  margin-top: 2rem;
  width: fit-content;
}
</style>
