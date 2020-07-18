<template>
  <div class="container-fluid my-15 py-10">
    <div class="container">
      <v-row>
        <v-col md="12">
          <v-carousel hide-delimiters cycle height="600" class="rounded-lg">
            <v-carousel-item
              v-for="(item, i) in items"
              :key="i"
              :src="item.src"
            >
            </v-carousel-item>
          </v-carousel>
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "https://i.ibb.co/ZmdTM02/DSCF0787-1.jpg"
        },
        {
          src: "https://i.ibb.co/3mMs84P/DSCF0806-1.jpg"
        },
        {
          src: "https://i.ibb.co/g3tsgcT/DSCF0791.jpg"
        },
        {
          src: "https://i.ibb.co/Rzd9ZmZ/DSCF0803-1.jpg"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.v-carousel {
  box-shadow: 0px 0px 50px;
}
</style>
