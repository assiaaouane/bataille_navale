<template>

    <div class="Plateau">

        <h1>BATAILLE NAVALE</h1>

        <table class="plateau">

            <tr v-for = "(verticale, index) in monPlateau[0]" :key="index">

                <td v-for="(horizontale, index2) in monPlateau[1]" :key="index2" @click = "getCoordonnees(index,index2)">
                    {{horizontale}} - {{verticale}}
                </td>

            </tr>
        </table>

        <div>
           <h2>plateau Vide</h2>
        </div>

        <table class="plateau2">
            <tr v-for = "x in 10" :key ='x'>

                <td v-for="y in 10" :key="y">

                </td>
            </tr>
        </table>

    </div>

</template>




<script>

    export default {
        name: "Plateau.vue",

        data: function () {
            return {
                monPlateau: [
                    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
                    ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']
                ]
            }
        },

    }

</script>




<style scoped>


    h1 {
        font-family: Stencil Std, fantasy ;
        font-weight: 400;
    }

    table {
        border: medium solid #000000;
        border: 1px solid black;

        width: 50%;
        background-color: #7597b8;
        color: white;
        margin: auto;
    }

    tr{
        border: 1px solid black;
        height: 50px
    }


    td{
        border: 1px solid black;
        height: 50px
    }



</style>