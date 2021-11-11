<template>
  <div id="app">
   <Polls v-bind:questions="questions"/>
  
  </div>
</template>

<script>
import Polls from '../components/Polls';
export default {
  name: 'Home',
  components: {
    Polls
  },
  data(){
    return {
      questions: [
        {
          id: 1,
          title: "Test 1",
          vote: 5
        },
        {
          id: 2,
          title: "Test 2",
          vote: 3
        },
        {
          id: 3,
          title: "Test 3",
          vote: 5
        }
      ]
    }
  }
}
</script>
