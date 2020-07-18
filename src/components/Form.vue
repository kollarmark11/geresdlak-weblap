<template>
  <div class="container-fluid">
    <v-row justify="center">
      <v-card width="600" class="my-15">
        <v-card-text>
          <form action="POST" name="contact" method="POST" netlify>
            <v-col md="12" class="ma-0 py-3">
              <input type="text" name="name" placeholder="Név" />

              <input type="text" name="name" placeholder="E-mail" />
              <textarea
                name="message"
                cols="30"
                rows="5"
                placeholder="Üzenet"
              ></textarea>

              <div class="button">
                <button type="submit">
                  Küldés
                </button>
              </div>
            </v-col>
          </form>
        </v-card-text>
      </v-card>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container-fluid {
  background-color: #6a1b9a;
}

input,
textarea {
  background-color: #e0e0e0;
  padding: 10px;
  margin: 20px;
  width: 500px;
  border-radius: 10px;
}

.label {
  margin-bottom: 20px;
}
.button {
  margin: 0 auto;
  text-align: center;
  button {
    background-color: #6a1b9a;
    padding: 10px 20px;
    color: #ffffff;
    border-radius: 10px;
  }
}
</style>
