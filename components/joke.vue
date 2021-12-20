<template>
  <nuxt-link :to="'jokes/' + id">
    <div class="joke">
      <p>{{ joke }}</p>
    </div>
  </nuxt-link>
</template>

<script>
export default {
  name: "Joke",
  props: ["joke", "id"],
};
</script>

<style>
.joke{
  padding: 1rem;
  border: 1px dotted #ccc;
  background-color: rgb(250, 250, 250);
  margin: 1rem 0;
}
p{
  color: black;
  font-size:18px;
}
</style>