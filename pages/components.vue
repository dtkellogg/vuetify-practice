<template>
<div>
  <h1>Vuetify Components</h1>
  <Buttons />
  <Cards />
  <Dividers />
  <Grid />
</div>
</template>

<script>
import Buttons from "~/components/Buttons"
import Cards from "~/components/Cards"
import Dividers from "~/components/Dividers"
import Grid from "~/components/Grid"
export default {
  components: {
    Buttons,
    Cards,
    Dividers,
    Grid
  },
  head() {
    return {
      title: "Vuetify Components"
    }
  }
}
</script>

<style>

</style>