<template>
<div>
  <h3>Buttons in their simplest form contain uppercase text, a slight elevation, hover effect, and a ripple effect on click.</h3>
  <v-btn>hello</v-btn>

  <h4>V-btn toggled</h4>
  <p>The v-btn-toggle component is a simple wrapper for v-item-group built specifically to work with v-btn.
  </p>
  <v-btn-toggle v-model="toggle_exclusive">
    <v-btn>
      <v-icon>mdi-format-align-left</v-icon>
    </v-btn>

    <v-btn>
      <v-icon>mdi-format-align-center</v-icon>
    </v-btn>

    <v-btn>
      <v-icon>mdi-format-align-right</v-icon>
    </v-btn>

    <v-btn>
      <v-icon>mdi-format-align-justify</v-icon>
    </v-btn>
  </v-btn-toggle>
  <p>Multiple</p>
  <v-btn-toggle
    v-model="toggle_multiple"
    dense
    background-color="primary"
    dark
    multiple
  >
    <v-btn>
      <v-icon>mdi-format-bold</v-icon>
    </v-btn>

    <v-btn>
      <v-icon>mdi-format-italic</v-icon>
    </v-btn>

    <v-btn>
      <v-icon>mdi-format-underline</v-icon>
    </v-btn>

    <v-btn>
      <v-icon>mdi-format-color-fill</v-icon>
    </v-btn>
  </v-btn-toggle>
</div>
</template>

<script>
export default {

}
</script>

<style>

</style>