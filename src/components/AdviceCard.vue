<template>
  <v-card :rounded="0">
    <v-card-title class="text-uppercase"
      ><v-icon size="x-large" color="black" start>{{
        `mdi-numeric-${index + 1}-circle`
      }}</v-icon>
      {{ advice.titre }}</v-card-title
    >

    <v-card-text class="ml-12 mr-12" style="max-height: 700px">
      <div
        style="width: 100%; height: 55px; overflow: hidden"
        v-html="advice.description"
      ></div>
    </v-card-text>
    <v-card-actions>
      <v-row justify="center">
        <v-col cols="auto" class="text-center pt-0">
          <v-btn variant="outlined">Plus d'informations</v-btn>
        </v-col>
      </v-row>
    </v-card-actions>
  </v-card>
</template>
<script >
export default {
  data() {
    return {

    }
  },
    props: {
    advice: Object,
    index: Number
  },
    mounted(){

  },
    methods: {

  }
}
</script>