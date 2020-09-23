<template>
  <div>
    <v-list class="list--maxwidth">
      <v-list-item>
        <v-list-item-content>N Orden</v-list-item-content>
        <v-list-item-content>{{ this.contenidoT1.num_orden }}</v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-content>Monto Orden</v-list-item-content>
        <v-list-item-content>{{ this.contenidoT1.monto }}</v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-content>Cant. Productos</v-list-item-content>
        <v-list-item-content>{{ this.contenidoT1.cant_productos }}</v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-content>Fecha Entrega</v-list-item-content>
        <v-list-item-content>{{ this.date }}</v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-content>Vendedor</v-list-item-content>
        <v-list-item-content>{{ this.contenidoT1.vendedor }}</v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-content>Estado</v-list-item-content>
        <v-list-item-content>{{ this.contenidoT1.estado }}</v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-content>Avance Preparación</v-list-item-content>
        <v-list-item-content>
          <v-progress-linear
            background-color="info"
            color="grey lighten-4"
            :value="this.advancePCT"
            height="10"
            rounded
            class="border-grey"
          ></v-progress-linear>
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </div>
</template>

<script>
export default {
  name: 'Tabs',
  props: {
    contenidoGeneral: Object,
    dateFixed: String, 
    advanceFixed: Number
  },
  data()
  {
    return {
      tab: null,
      contenidoT1: this.contenidoGeneral,
      date: this.dateFixed,
      advancePCT: this.advanceFixed,
    }
  },
  computed: {
  },
}
</script>

<style lang="scss" scoped>
.border-grey {
  border: solid 1px grey;
}
.list--maxwidth {
  max-width: 450px;
}
</style>