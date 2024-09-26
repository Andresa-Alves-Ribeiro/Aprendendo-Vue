<template>
    <div class="componente">
        <h1>Componente Com Dados Não Alteráveis</h1>
        <p>Nome: {{ nomeProduto }} - {{ codigoProduto }}</p>
    </div>
</template>

<script setup>
// TRABALHAR COM DADOS QUE NÃO PODEM SER ALTERADOS
const nomeProduto = "Caderno";
const codigoProduto = "#987"
</script>

<!-- 
<script>
// NÃO PODE USAR ARROW FUNCTION

// COMPOSITION API
export default {
    setup: function () {
        nomeProduto = 'Caneta'
        codigoProduto = '#123'
        return {
            nomeProduto,
            codigoProduto
        }
    }
}
</script> 
-->