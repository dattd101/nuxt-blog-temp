<template>
  <div>
    <SidebarVue />
    <v-container>
      <v-card>
        <v-card-text class="d-flex justify-space-between align-center">
          <v-card-title> Category ( 33 ) </v-card-title>
          <v-card-actions>
            <nuxt-link to="/admin/create-category">
              <v-btn color="red lighten-2">New </v-btn>
            </nuxt-link>
          </v-card-actions>
        </v-card-text>
        <hr />

        <v-card-subtitle>
          <v-simple-table>
            <template v-slot:default>
              <thead>
                <tr>
                  <th class="text-left">Id</th>
                  <th class="text-left">Category</th>
                  <th class="text-left">Status</th>
                  <th class="text-left">Edit</th>
                  <th class="text-left">Delete</th>
                </tr>
              </thead>
              <tbody>
                <tr v-for="(item, index) in 5" :key="index">
                  <td class="text-left">{{ index + 1 }}</td>
                  <td class="text-left">category {{ index + 1 }}</td>
                  <td class="text-left">1</td>
                  <td class="text-left">
                    <nuxt-link to="/admin/update-category/1">
                      <v-btn
                        text
                        class="ma-2"
                        @click="edit_dialog = true"
                        variant="text"
                        color="blue"
                      >
                        <v-icon color="blue darken-3"> mdi-pencil</v-icon>
                      </v-btn>
                    </nuxt-link>
                  </td>
                  <td class="text-left">
                    <v-btn text class="ma-2" variant="text" color="red">
                      <v-icon color="red darken-3"> mdi-delete</v-icon>
                    </v-btn>
                  </td>
                </tr>
              </tbody>
            </template>
          </v-simple-table>
        </v-card-subtitle>
      </v-card>
    </v-container>
  </div>
</template>
<script>
import SidebarVue from "../../components/admin/Sidebar.vue";

export default {
  name: "CategoryPage",
   head(){
  return{
   title:'Category',
  }
  },

  components: {
    SidebarVue,
  },
};
</script>
<style>
</style>