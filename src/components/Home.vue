<template>
  <Layout>
    <template #header>
      <Header></Header>
    </template>
    <template #resume>
      <Resumen :label="'Ahorro total'" :total-amount="10000000" :amount="amount" />
    </template>
    <template>
      <Movements />
    </template>
  </Layout>
</template>

<script>
import Layout from "./Layout.vue";
import Header from "./Header.vue";
import Resumen from "./Resumen/Index.vue";
import Movements from "./Movements.vue";
export default {
  components: {
    Layout,
    Header,
    Resumen,
    Movements,
  },
  data() {
    return {
      amount: null
    }
  }
};
</script>
