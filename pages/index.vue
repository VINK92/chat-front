<template>
  <div>
    <div class="container">
      <img :src="srcTitleImg" alt="Patric" width="300" height="300">
      <div class="titleContainer">
        <h1 class="title">{{title}}</h1>
        <p>{{subTitle}}</p>
      </div>
    </div>
    <Message/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      title: 'Chat bots 2.0',
      subTitle: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
      srcTitleImg: '/static/images/bigchatbot.jpg',
    }
  }
})
</script>

<style>
#__nuxt {
  font-family: "Open Sans";
  font-size: 14px;
}
.container {
  display: flex;
  flex-direction: row;
}
.titleContainer {
  display: flex;
  flex-direction: column;
}
.title {
  color: #333333;
}
</style>
