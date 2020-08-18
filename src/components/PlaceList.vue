<template>
  <v-container>
    <v-row class="text-center">
      <v-col
        v-for="place in arPlace"
        :key="place"
        cols="4"
      >
        <v-card
            class="mx-auto"
            max-width="200"
            outlined
            hover
        >
            <v-list-item three-line>
                <v-list-item-content>
                    <div class="overline mb-4">Место №{{ place }}</div>
                    <v-list-item-title class="headline mb-1">{{ place }}</v-list-item-title>
                    <v-list-item-subtitle>Место свободно</v-list-item-subtitle>
                </v-list-item-content>
            </v-list-item>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
    name: 'PlaceList',
    data: () => ({
        arPlace: [1, 2, 3, 4, 5, 6],
    }),

}
</script>

<style>

</style>