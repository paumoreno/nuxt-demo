<template>
  <div class="Planets">
    <div class="Planets__phrase" @click="nextName">Hello {{name}}!</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      names: [
        'Mercury',
        'Venus',
        'Earth',
        'Mars',
        'Jupiter',
        'Saturn',
        'Uranus',
        'Neptune'
      ],
      nameIndex: 0
    }
  },
  computed: {
    name() {
      return this.names[this.nameIndex]
    }
  },
  methods: {
    nextName() {
      this.nameIndex =
        (this.nameIndex === this.names.length - 1) ? 0 : this.nameIndex + 1
    }
  }
}
</script>

<style>
.Planets {
  text-align: center;
  background-color: #080c1d;
  color: white;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.Planets__phrase {
  font-size: 2em;
  cursor: pointer;
}
</style>

