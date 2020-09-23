<template>
  <div>
    <!-- breadcrumb -->
    <h1>Monitor de Órdenes</h1>

    <v-tabs v-model="tab">
      <v-tab
        v-for="item in tabNames"
        :key="item"
      >
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item>
        <orden-general
          :contenidoGeneral="this.orden"
          :advanceFixed="this.getFixedAdvance"
          :dateFixed="this.getFixedDate"
        ></orden-general>
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
import OrdenGeneral from '@/components/OrdenGeneral'
import { mapState, mapGetters } from 'vuex'

export default {
  name: 'DetalleOrden',
  components: {
    OrdenGeneral,
  },
  data() 
  {
    return {
      tab: null,
      tabNames: [
        'General',
        'Datos Cliente',
        'Productos'
      ],
    }
  },
  computed: {
    ...mapState([
      'orden',
      'cliente',
      'productos'
    ]),
    ...mapGetters([
      'getFixedAdvance',
      'getFixedDate'
    ])
  }
}
</script>