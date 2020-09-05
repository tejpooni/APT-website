<template>
    <div class="inlinecards">

        <v-card class="mx-auto" width="500" height="400" hover>
            <v-img class="white--text align-end" height="400px" src="../../assets/img/Fitnesstest.png" >
                <v-card-title>Fitness Test</v-card-title>
            </v-img>
        </v-card>


        <v-card class="mx-auto" width="500" height="400" hover>
            <v-img class="white--text align-end" height="400px" src="../../assets/img/Mealplan.jpg" >
                <v-card-title>Meal Plan</v-card-title>
            </v-img>
        </v-card>


        <v-card class="mx-auto" width="500" height="400" hover>
            <v-img class="white--text align-end" height="400px" src="../../assets/img/workout.jpg" >
                <v-card-title>Workouts</v-card-title>
            </v-img>
        </v-card>


        <v-card class="mx-auto" width="500" height="400" hover>
            <v-img class="white--text align-end" height="400px" src="../../assets/img/store.jpeg" >
                <v-card-title>Shop</v-card-title>
            </v-img>
        </v-card>

    </div>


</template>

<script>
    export default {
        name: "Section"
    }
</script>

<style scoped>
    .inlinecards{
        display: grid;
        grid: 400px / auto auto;
        grid-gap: 20px;
    }
</style>