<template >
  <div class="bg__blue">
    <v-container class="mt-10">
      <v-row class="my-5">
        <v-col xl="4" lg="4" md="4" sm="6" xs="12">
          <h3 class="text--white">About Website</h3>
          <p class="text--white">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt,
            repudiandae modi. Quaerat optio magnam ipsam velit! Laudantium
            exercitationem harum quis, rem a quos earum! Neque nobis vitae omnis
            quidem. At.
          </p>
          <v-btn
            color="primary"
            style="color: white !important"
            class="btn__border"
            text
            >About Me</v-btn
          >
        </v-col>
        <v-col xl="4" lg="4" md="4" sm="6" xs="12">
          <h3 class="text--white">Quick Links</h3>
          <ul>
            <li>Home</li>
            <li>Home</li>
            <li>Home</li>
          </ul>
        </v-col>
        <v-col xl="4" lg="4" md="4" sm="6" xs="12">
          <h3 class="text--white">Subscribe For News Latter</h3>

          <form action="">
            <v-text-field
              label="Enter Category"
              class="form__control"
              hide-details="auto"
            >
            </v-text-field>

            <v-btn
              color="success"
              text
              class="login__btn"
              style="border: 1px solid blue"
              @click="edit_dialog = false"
            >
              Update</v-btn
            >
          </form>
          <v-btn style="margin-left: 2px; background-color: blue">
            <v-icon>mdi-facebook</v-icon>
          </v-btn>
          <v-btn style="margin-left: 2px; background-color: black">
            <v-icon>mdi-github</v-icon>
          </v-btn>
          <v-btn style="margin-left: 2px; background-color: red">
            <v-icon>mdi-instagram</v-icon>
          </v-btn>
          <v-btn style="margin-left: 2px; background-color: lightblue">
            <v-icon>mdi-twitter</v-icon>
          </v-btn></v-col
        >
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  name: "FooterCamp",
  data: () => ({
    model: 0,
  }),
};
</script>
<style>
</style>