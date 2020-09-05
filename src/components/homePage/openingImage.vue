<template>
    <div class="gay">
        <v-parallax class="opening" height="1000" src="../../assets/landing.jpg">
            <v-row
                    align="center"
                    justify="center"
            >
                <v-col class="text-center" cols="5">
                    <v-img class="logo" src="../../assets/logo.png"> </v-img>
                </v-col>
                <v-col class="text-center" cols="8">
                    <v-btn  relative
                            center
                            fab
                    >
                        <v-icon size="100" color="blue"> {{icon_name}} </v-icon>
                    </v-btn>
                </v-col>
            </v-row>
        </v-parallax>
    </div>


</template>


<script>
    export default {
        name: "openingImage",
        data() {
            return {
            icon_name: "mdi-arrow"
            }
        }

    }
</script>

<style scoped>

    .gay{
height: 100vh;
    }
.opening {

    height: 100vh;
    background-position: left bottom;
    background-size: cover;
    text-align: center;


    display: flex;
    flex-direction: column;
    justify-content: center;

}
.logo {
    margin-left: auto;
    margin-right: auto;
    width: 30em;
    filter: drop-shadow(0 0 20px #000);
}
</style>

