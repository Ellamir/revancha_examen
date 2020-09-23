<template>
  <div>
    <!-- breadcrumb -->
    <h1>Monitor de Órdenes</h1>

    <tabs
      :tabNames="this.tabNames"
      :contentTab1="this.orden"
      :advancePercentage="this.getFixedAdvance"
      :dateFixed="this.getFixedDate"
    ></tabs>
  </div>
</template>

<script>
import Tabs from '@/components/Tabs'
import { mapState, mapGetters } from 'vuex'

export default {
  name: 'DetalleOrden',
  components: {
    Tabs,
  },
  data() 
  {
    return {
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