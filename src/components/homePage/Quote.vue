<template>
    <div v-on:scroll="scrollFunction"  class="vision">
        <p class="black--text" id="statement">We are dedicated to providing you with the necessary tools to reach your fitness goals.
            Our team strongly believes that with proper guidance, anyone can be successful. <br>
            <span>Start right with APT today!</span>
        </p>
        <div id="line"></div>
        <p class="black--text" id="vision"> The <span class="red--text">APT</span> Vision.</p>
    </div>
</template>

<script>
    export default {
        name: "quote",
        created() {
            window.addEventListener('scroll', this.handleScroll);
        },
        destroyed() {
            window.removeEventListener('scroll', this.handleScroll)
        },
        methods: {
            handleScroll (event) {
                /*
                if (window.pageYOffset >= 0.8*screen.availHeight){
                   document.getElementById("nb").style.top = "0em";
                }else{
                   document.getElementById("nb").style.top = "-4em";
                }
            */
                console.log(event)
                if (window.pageYOffset >= 0.15*screen.availHeight){
                    document.getElementById("statement").style.right = "52%";
                    document.getElementById("statement").style.opacity = 1;
                    document.getElementById("vision").style.left = "52%";
                    document.getElementById("vision").style.opacity = 1;
                    document.getElementById("line").style.opacity = 1;
                    document.getElementById("line").style.height = "18vw";
                }else{
                    document.getElementById("statement").style.right = "40%";
                    document.getElementById("statement").style.opacity = 0;
                    document.getElementById("vision").style.left = "40%";
                    document.getElementById("vision").style.opacity = 0;
                    document.getElementById("line").style.opacity = 0;
                    document.getElementById("line").style.height = "0vw";
                }
            }
        }
    }


</script>

<style scoped>

    .vision{
        height: 30vw;
        position: relative;
        background-color: #ffffff;
    }
    #vision {
        font-family: Sen;
        font-weight: 800;
        position: absolute;
        transform: translateY(-50%);
        top: 50%;

        left: 45%;
        font-size: 4vw;
        transition: 1s;
    }

    #statement {

        position: absolute;
        transform: translateY(-50%);
        top: 50%;
        right: 45%;
        width: 35%;

        font-size: 1.5vw;
        text-align: justify;
        text-align-last: right;
        transition: 1s;
        line-height: 160%;

    }

    #statement span {

        font-weight: 800;
    }
    #line {
        position:absolute;
        border-left: .5vw solid #ac0000;
        border-radius: .5vw;
        height: 18vw;
        top: 50%; left: 50%;
        transform: translate(-50%, -50%);
        transition: 1s;
    }


</style>