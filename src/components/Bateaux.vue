<template>
    <div class="Bateaux">

        <table class="table table-bordered">

            <caption>Bateaux</caption>

            <thead>
            <tr>
                <th>Nom</th>
                <th>Size</th>

            </tr>
            </thead>
            <tbody >
            <tr v-for="Bateau in Bateaux" :key="Bateau">
                <td>{{ Bateau.Nom }}</td>
                <td>{{ Bateau.size }}</td>
            </tr>
            </tbody>
        </table>


    </div>
    
</template>

<script>

    export default {
        name: "Bateaux.vue",

        data: function(){
            return{
                Bateaux:[
                    {Nom:"Porte-avion",id:8,size:5 },
                    {Nom:"Croiseur",id:7,size:4 },
                    {Nom:"Contre-torpilleur",id:6,size:3},
                    {Nom:"Sous-marin",id:5,size:3},
                    {Nom:"Torpilleur",id:4,size:2}
                ]

            }

        }
    }
</script>

<style scoped>
    table {
        border: medium solid #000000;
        border: 1px solid black;
        border-collapse: collapse;

    }
th{

    border: 1px solid black;
}
</style>
