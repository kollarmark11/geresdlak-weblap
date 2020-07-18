<template>
  <div class="home">
    <Slider />
    <Welcome />
    <Carousel />
    <TeamMembers />
    <Form />
  </div>
</template>

<script>
// @ is an alias to /src
import Slider from "../components/Slider.vue";
import Welcome from "../components/Welcome.vue";
import Carousel from "../components/Carousel.vue";
import TeamMembers from "../components/TeamMembers.vue";
import Form from "../components/Form.vue";

export default {
  components: {
    Slider,
    Welcome,
    Carousel,
    TeamMembers,
    Form
  }
};
</script>
