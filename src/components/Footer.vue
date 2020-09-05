<template>
    <v-footer
            color="red darken-3"
            padless
    >
        <v-row
                justify="center"
                no-gutters
        >
            <v-btn
                    v-for="link in links"
                    :key="link"
                    color="white"
                    text
                    rounded
                    class="my-2"

            >
               <a class="links" :href="link.link"  >{{ link.name }}</a>
            </v-btn >
            <v-btn color="white"
                   text
                   rounded
                   class="my-2">

                <router-link class="links" to="/about">Contact Us</router-link>
            </v-btn>

            <v-col
                    class="red darken-4 py-4 text-center white--text"
                    cols="12"
            >
                {{ new Date().getFullYear() }} — <strong>APT</strong>
            </v-col>
        </v-row>
    </v-footer>
</template>

<script>
    export default {
        name: "Footer",
        data: () => ({
            links: [
                { name:'Home',
                  link: "/home"}  ,
                { name:'Workouts',
                  link: "/workouts" },
                { name:'APP',
                    link: "/apps" },
                { name:'Instagram',
                    link: "https://www.instagram.com/aptgains/" },
                { name:'Facebook',
                    link: "https://www.facebook.com/Aptgains-100102434977814" },


            ],
        }),
    }
</script>

<style scoped>
    .links {
        color: inherit; /* blue colors for links too */
        text-decoration: inherit; /* no underline */
    }


</style>