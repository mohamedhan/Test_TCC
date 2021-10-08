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
 data() {
    return {
      fields: [
        { key: "lastName", label: "Last Name" },
        { key: "firstName", label: "First Name" },
        { key: "email", label: "Email" },
        { key: "Actions", label: "Actions" },
      ],
    };
  },
 
  methods: {
    delete(id) {
      console.log("deleteeeeeeee", id);
      this.$emit("delete-person", id);
    },
  },

};
</script>
