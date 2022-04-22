<!-- Please remove this file from your project -->
<template>
  <div class="messageContainer">
    <span>{{messageTime}}</span>
  </div>
</template>

<script lang="ts">

import Vue from 'vue'
import moment from 'moment';
export default Vue.extend({
  props() {
    return {
      variant: {
        type: String,
        dafault: 'grey',
      }
    }
  },
  data() {
    return {
      messageTime: moment().format('LT')
    }
  }
})

</script>

<style scoped>
.messageContainer {
  width: 800px;
  height: 100px;
  background: rgb(243, 242, 242);
  box-shadow: 4px 4px 8px 0px rgba(34, 60, 80, 0.2);
  border-radius: 5px;
}
</style>
