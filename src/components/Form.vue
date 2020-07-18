<template>
  <div class="container-fluid">
    <v-row justify="center">
      <form name="contact" method="POST" data-netlify="true">
        <v-form ref="form" v-model="valid" lazy-validation>
          <v-col md="10">
            <v-text-field
              v-model="lastname"
              label="Vezetéknév"
              :rules="nameRules"
              r
              equired
              width="100"
            ></v-text-field>

            <v-text-field
              v-model="lastname"
              label="Keresztnév"
              :rules="nameRules"
              r
              equired
            ></v-text-field>

            <v-text-field
              v-model="lastname"
              label="Email"
              :rules="nameRules"
              r
              equired
            ></v-text-field>
          </v-col>
          <v-btn type="submit">Küldés</v-btn>
        </v-form>
      </form>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nameRules: [
        v => !!v || "Kötelező mező!",
        v => (v && v.length <= 30) || "Name must be less than 10 characters"
      ],
      emailRules: [
        v => !!v || "Kötelező mező!",
        v => /.+@.+\..+/.test(v) || "E-mail must be valid"
      ]
    };
  }
};
</script>
