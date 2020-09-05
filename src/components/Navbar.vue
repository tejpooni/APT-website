<template>
    <v-app-bar
            app
            color="red darken-4"
            scroll-target="#scrolling-techniques6"
            src="assets/logo.png"



    >
        <div class="d-flex align-center">
            <router-link to="/"><v-img
                    alt="APT LOGO"
                    class="shrink mr-2"
                    contain
                    src="../assets/logo.png"
                    transition="scale-transition"
                    width="40"
            /></router-link>

            <div>
                <v-spacer>   </v-spacer>
                <div class="v-tabs--centered">
                    <v-btn small> Fitness test</v-btn>
                </div>

            </div>
        </div>
        <div>
            <v-spacer>   </v-spacer>
            <div class="v-tabs--centered">
                <v-btn small> Meal Plans</v-btn>
            </div>

        </div>

        <div>
            <v-spacer>   </v-spacer>
            <div class="v-tabs--centered">
                <v-btn small> workouts</v-btn>
            </div>

        </div>

        <div>
            <v-spacer></v-spacer><v-spacer></v-spacer>
            <div class="v-tabs--centered">
                <v-btn small>Shop</v-btn>
            </div>

        </div>


        <v-spacer></v-spacer>
        <div class="align-right">
            <a class="links" target="_blank" href="https://www.instagram.com/aptgains/"><v-btn icon>
                <v-icon size="40" color="white">mdi-instagram</v-icon>
        </v-btn></a>
            <a class="links" target="_blank" href="https://www.facebook.com/Aptgains-100102434977814"><v-btn icon>
                <v-icon size="40" color="white">mdi-facebook</v-icon>
            </v-btn></a>


        </div>

    </v-app-bar>
</template>

<script>
    export default {
        name: "Navbar"
    }
</script>

<style scoped>
    .links {
        color: inherit; /* blue colors for links too */
        text-decoration: inherit; /* no underline */
    }

</style>