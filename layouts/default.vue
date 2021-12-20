<template>
  <div>
    <AppHeader />
    <main>
      <Nuxt />
    </main>
    <footer>
        <div>
            <h4>Made with Love by Moiez Malik</h4>
        </div>
    </footer>
  </div>
</template>

<script>
import AppHeader from "../components/AppHeaders.vue";

export default {
  components: {
    AppHeader,
  },
};
</script>

<style>
html{
   margin:0;
   padding:0;
   height:100%;
}
body {
   min-height:100%;
   position:relative;
}
main {
   padding:10px;
   padding-bottom:60px;   /* Height of the footer */
}
footer {
   position:absolute;
   bottom:0;
   width:100%;
   padding-top: 36px;   /* Height of the footer */
   text-align: center;
}
</style>