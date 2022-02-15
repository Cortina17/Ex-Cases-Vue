<template>
  <v-container>
    <v-row class="text-center">
      <h1>Grades</h1>
    </v-row>
    <v-row>
      <h3>Introduce your mark, and I'll tell you your grade.</h3>
      <input type="text" id="input-txt" />
      <button>Send mark</button>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Grades",

  data: () => ({}),
};
</script>
