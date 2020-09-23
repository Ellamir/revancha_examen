<template>
  <div>
    <v-tabs v-model="tab" align-with-title>
      <v-tab
        v-for="item in items"
        :key="item"
      >
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item>
        <v-list dense class="list--maxwidth">
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
      </v-tab-item>
      <v-tab-item>
        b
      </v-tab-item>
      <v-tab-item>
        c
      </v-tab-item>
    </v-tabs-items>
  </div>
</template>

<script>
export default {
  name: 'Tabs',
  props: {
    tabNames: Array,
    contentTab1: Object,
    contentTab2: Object,
    contentTab3: Object,
    advancePercentage: Number,
    dateFixed: String
  },
  data()
  {
    return {
      tab: null,
      items: this.tabNames,
      contenidoT1: this.contentTab1,
      contenidoT2: this.contentTab2,
      contenidoT3: this.contentTab3,
      advancePCT: this.advancePercentage,
      date:this.dateFixed
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