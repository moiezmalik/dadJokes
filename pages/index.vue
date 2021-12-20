<template>
<div class="container">
  <h2>Welcome to the best Dad Jokes on the web</h2>
</div>
</template>

<script>
export default {
  name: 'IndexPage',
  head(){
        return {
            title: 'Welcome to Dad Jokes',
            meta: [
                {
                    hid: 'description',
                    name: 'description',
                    content: 'Best place for Corny dad jokes'
                }
            ]
        }
    }
}
</script>
