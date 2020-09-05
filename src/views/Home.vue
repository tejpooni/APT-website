<template>
  <div>
    <div>
   <opening-image/>
  </div>
     <quote/>
        <Section />
           <athletes/>

    </div>


</template>

<script>
// @ is an alias to /src
import openingImage from "../components/homePage/openingImage"
import Quote from "../components/homePage/Quote";
import Athletes from "../components/homePage/athletes";
import Section from "../components/homePage/Section";

export default {
  name: 'Home',
  components: {
      Athletes,
      Quote,
      openingImage,
      Section

  }
}
</script>

<style scoped>


</style>
