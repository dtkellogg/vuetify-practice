<template>
  <div>
    <h1>Grid</h1>

    <h2>v-container</h2>
    <p>v-container provides the ability to center and horizontally pad your site’s contents. You can also use the fluid prop to fully extend the container across all viewport and device sizes. Maintains previous 1.x functionality in which props are passed through as classes on v-container allowing for the application of helper classes (such as ma-#/pa-#/fill-height) to easily be applied</p>

    <h3>Vertical Alignment</h3>
    
    <v-container
      v-for="align in alignments"
      :key="align"
      class="grey lighten-5 mb-6"
    >
      <v-row
        :align="align"
        no-gutters
        style="height: 150px;"
      >
        <v-col
          v-for="n in 3"
          :key="n"
        >
          <v-card
            class="pa-2"
            outlined
            tile
          >
            One of three columns
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="grey lighten-5">
      <v-row
        no-gutters
        style="height: 150px;"
      >
        <v-col
          v-for="align in alignments"
          :key="align"
          :align-self="align"
        >
          <v-card
            class="pa-2"
            outlined
            tile
          >
            One of three columns
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <h3>Horizontal Alignment</h3>

    <v-container class="grey lighten-5">
    <v-row
      v-for="j in justify"
      :key="j"
      :justify="j"
    >
      <v-col
        v-for="k in 2"
        :key="k"
        md="4"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          One of two columns
        </v-card>
      </v-col>
    </v-row>
  </v-container>


    <h2>v-col</h2>
    <p>v-col is a content holder that must be a direct child of v-row. This is the 2.x replacement for v-flex in 1.x.</p>
    <h2>v-row</h2>
    <p>v-row is a wrapper component for v-col. It utilizes flex properties to control the layout and flow of its inner columns. It uses a standard gutter of 24px. This can be reduced with the dense prop or removed completely with no-gutters. This is the 2.x replacement for v-layout in 1.x.</p>
    <h2>v-spacer</h2>
    <p>v-spacer is a basic yet versatile spacing component used to distribute remaining width in-between a parents child components. When placing a single v-spacer before or after the child components, the components will push to the right and left of its container. When more than one v-spacer's are used between multiple components, the remaining width is evenly distributed between each spacer.
    </p>
  </div>
</template>

<script>
export default {
  data: () => ({
    alignments: [
      'start',
      'center',
      'end',
    ],
    justify: [
      'start',
      'center',
      'end',
      'space-around',
      'space-between',
    ],
  }),
}
</script>

<style>

</style>