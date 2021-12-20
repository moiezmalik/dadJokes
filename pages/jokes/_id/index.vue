<template>
  <div class="container">
    <div class="row">
      <div class="col-md-8 offset-md-2">
        <div class="card">
          <div class="card-body">
            <nuxt-link to="/jokes" class="btn btn-info">Back to Jokes</nuxt-link>
          </div>
          <div class="card-body">
            <h2>{{ joke }}</h2>
            <small>Joke ID: {{ $route.params.id }}</small>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      joke: {},
    };
  },
  async created() {
    const config = {
      headers: {
        Accept: "application/json",
      },
    };
    try {
      const res = await axios.get(
        `https://icanhazdadjoke.com/j/${this.$route.params.id}`,
        config
      );
      this.joke = res.data.joke;
    } catch (err) {
      console.log(err);
    }
  },
  head() {
    return {
      title: this.joke,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Best place for Corny dad jokes",
        },
      ],
    };
  }
};
</script>

<style>
</style>