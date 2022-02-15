<template>
  <v-container>
    <v-row class="text-center">
      <h1>Grades</h1>
    </v-row>
    <v-row>
      <h3>Introduce your mark, and I'll tell you your grade.</h3>
      <input v-model="" type="text" id="input-txt" />
      <button v-on:click="grades()">Send mark</button>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Grades",

  data: () => ({}),
  methods: {
    grades(num) {
      if (num >= 0 && num <= 10) {
        return num >= 9
          ? "Outstanding"
          : num < 9 && num >= 7
          ? "Remarkable"
          : num < 7 && num >= 5
          ? "Suficient"
          : num < 5 && num >= 3
          ? "Insuficient"
          : "Too poor";
      }
      return "Enter a number between 0 and 10";
    },
  },
};
</script>
