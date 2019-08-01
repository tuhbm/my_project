<template>
    <div class="calculator--component">
        <table border="1">
            <tr>
                <td colspan="4">
                    <input type="text" id="display">
                </td>
            </tr>
            <tr>
                <td colspan="4">
                    <input type="text" id="result">
                </td>
            </tr>
            <tr>
                <td colspan="3">AC</td>
                <td>/</td>
            </tr>
            <tr>
                <td>7</td>
                <td>8</td>
                <td>9</td>
                <td>*</td>
            </tr>
            <tr>
                <td>4</td>
                <td>5</td>
                <td>6</td>
                <td>-</td>
            </tr>
            <tr>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>+</td>
            </tr>
            <tr>
                <td colspan="2">0</td>
                <td>.</td>
                <td>=</td>
            </tr>
        </table>
    </div>
</template>

<script>
    export default {
        name: "CalculatorContent"
    }
</script>

<style scoped>
    .calculator--component {
        width: 50%;
        margin:5em auto;
        text-align:center;
    }
    .calculator--component table {
        width: 100%;
        border: 1px solid #000;
        border-collapse: collapse;
    }

    .calculator--component td {
        padding: 5px 10px;
        border: 1px solid #000;
        text-align: center;
    }

    .calculator--component input {
        text-align: right;
        border: none;
    }

    .calculator--component input:focus {
        outline: none;
    }
</style>