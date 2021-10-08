<template>
  <v-app>
     <UsersList />
  </v-app>
</template>

<script>
import UsersList from "./components/UsersList.vue"
export default {
  name: "App",

  components: {
    UsersList
  },

};
</script>
