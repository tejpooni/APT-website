<template>
    <div>
        <h1 class="text-center" >Our Athletes</h1>
        <h1>&nbsp;</h1>
        <v-sheet
                class="mx-auto"
                elevation="8"
                max-width="1200"
        >
            <v-slide-group
                    v-model="model"
                    class="pa-4"
                    :prev-icon="prevIcon ? 'mdi-minus' : undefined"
                    :next-icon="nextIcon ? 'mdi-plus' : undefined"
                    :multiple="multiple"
                    :mandatory="mandatory"
                    :show-arrows="showArrows"
                    :center-active="centerActive"
            >
                <v-slide-item
                        v-for="athlete in athletics"
                        :key="athlete"

                >
                    <v-card

                        class="ma-4"
                        height="300"
                        width="300"
                        @click="toggle"
                        hover>
                        <v-card-text>{{athlete.type}}</v-card-text>
                        <v-card-title>{{athlete.name}}</v-card-title>
                        <v-card-text>{{athlete.handle}}</v-card-text>
                        <v-card-text >{{athlete.description}}</v-card-text>
                           <v-row
                                class="fill-height"
                                align="center"
                                justify="center"
                        >

                        <v-scale-transition>









                </v-scale-transition>
                        </v-row>
                    </v-card>
                </v-slide-item>
            </v-slide-group>
        </v-sheet>


    </div>
</template>

<script>
    export default {
        name: "athletes",
        data: () => ({
            model: null,
            multiple: false,
            mandatory: false,
            showArrows: true,
            prevIcon: false,
            nextIcon: false,
            centerActive: false,
            athletics: [
                {
                    name: "Gaintain Fitness",
                    img: "../../assets/img/gaintain.png",
                    handle: "@gaintainfitness",
                    type: "Personal Trainer",
                    description: "Gaintain Fitness better known as Tahmeed Hossain is a" +
                        " CFES certified weight trainer. Currently based in Kelowna B.C."

                },
                {
                    name: "Jamal",
                    handle: "@jamal.ahmed876",
                    type: "Personal Trainer",
                    description: "Gaintain Fitness better known as Tahmeed Hossain is a" +
                        " CFES certified weight trainer. Currently based in Kelowna B.C."

                },
                {
                    name: "Zafeer",

                    handle: "@zafeer63",
                    type: "Personal Trainer",
                    description: "Gaintain Fitness better known as Tahmeed Hossain is a" +
                        " CFES certified weight trainer"

                },
                {
                    name: "Humza",
                    img: "../../assets/img/gaintain.png",
                    handle: "@humzarai",
                    type: "Personal Trainer",
                    description: "Gaintain Fitness better known as Tahmeed Hossain is a" +
                        " CFES certified weight trainer. Currently based in Kelowna B.C."

                },
                {
                    name: "Husnain",

                    handle: "@husnain_nawaz24",
                    type: "Personal Trainer",
                    description: "Gaintain Fitness better known as Tahmeed Hossain is a" +
                        " CFES certified weight trainer. Currently based in Kelowna B.C."

                },
                {
                    name: "Usman",

                    handle: "@uzimankhan",
                    type: "Personal Trainer",
                    description: "Gaintain Fitness better known as Tahmeed Hossain is a" +
                        " CFES certified weight trainer. Currently based in Kelowna B.C."

                },
            ]
        }),

    }
</script>

<style scoped>


</style>