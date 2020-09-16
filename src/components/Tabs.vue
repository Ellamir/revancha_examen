<template>
  <div>
    <v-tabs v-model="tab">
      <v-tab>General</v-tab>
      <v-tab>Item Two</v-tab>
      <v-tab>Item Three</v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item></v-tab-item>
    </v-tabs-items>
  </div>
</template>

<script>
export default {
  name: 'Tabs',
  data()
  {
    return {
      tab: null,
    }
  }
}
</script>