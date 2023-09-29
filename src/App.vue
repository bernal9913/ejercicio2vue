<template>
  <div>
    <user-card :user="userData" />
  </div>
</template>

<script>
import UserCard from "./UserCard.vue";

export default {
  components: {
    UserCard
  },
  data() {
    return {
      userData: {
        name: "Carlos Bernal",
        age: 23,
        status: "Activo"
      }
    };
  }
};
</script>
