<template>
  <button @click="initBtn">{{ buttonText }}<img class="icon" v-if="icon_path" :src="icon_path" alt="icon"></button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    buttonText: String,
    icon_path: String
  },

  data() {
    return {
    }
  },

  methods: {
    initBtn() {
      this.$emit('init-button', true);
    }
  },

  mounted() {

  }
}
</script>

<style scoped>
button {
  display: flex;
  background-color: var(--accent);
  color: black;
  border-radius: 15px;
  padding: 0 12px 0 12px;
  border-color: black;
  cursor: pointer;
  align-items: center;
  justify-content: center;
}

.icon {
  width: 30px;
}
</style>