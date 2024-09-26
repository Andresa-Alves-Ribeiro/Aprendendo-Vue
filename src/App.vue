<script setup>
import FirstComponent from "./components/FirstComponent.vue"
import ComDados from "./components/ComDados.vue"
import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue"
import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue"
import DataBinding from "./components/DataBinding.vue"
import ComProps from "./components/ComProps.vue"

</script>

<template>
  <header>Header</header>
  <FirstComponent />
  <ComDados />
  <ComDadosReativosNaoPrimitivos />
  <ComDadosReativosPrimitivos />
  <DataBinding />
  <ComProps item="Apontador" :preco="13.50" />
</template>
