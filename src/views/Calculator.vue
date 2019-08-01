<template>
    <div class="calculator">
        <h1>This is calculator</h1>
        <calculator-content></calculator-content>
    </div>
</template>

<script>
    import CalculatorContent from '../components/calculator/CalculatorContent'

    export default {
        name: 'calculator',
        components: {
            CalculatorContent
        }
    }
</script>

<style scoped>
    .calculator {
        text-align: center;
    }
</style>
