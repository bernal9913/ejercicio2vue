<template>
  <div class="user-card">
    <div class="card">
      <div class="card-body">
        <img src="https://www.w3schools.com/howto/img_avatar.png" alt="Avatar" style="width:100%">
        <h5 class="card-title">{{ user.name }}</h5>
        <p class="card-text">Edad: {{ user.age }}</p>
        <p class="card-text">Estado: {{ user.status }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    user: {
      type: Object,
      required: true
    }
  }
};
</script>

<style>
.user-card {
  margin: 20px;
}

.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  border-radius: 5px; /* 5px rounded corners */
}

.card-title {
  font-size: 1.25rem;
  margin-bottom: 0.5rem;
}

.card-text {
  font-size: 1rem;
  margin-bottom: 0.25rem;
}
/* Add rounded corners to the top left and the top right corner of the image */
img {
  max-height: 300px;
  width: auto;
  border-radius: 5px 5px 0 0;
}
</style>
