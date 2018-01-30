<template>
  <div class="wrapper">
    <image :src="logo" class="logo"></image>
    <text class="greeting">The environment is ready!2</text>
    <text class="message">Now, let's use Vue.js to build your Weex app.</text>
  </div>
</template>

<script>
  const animation = weex.requireModule('animation');
  console.log(animation.transition) // check 
  
//   setTimeout(()=>{
//     const animation = weex.requireModule('animation');
//     console.log(animation.transition) // ok 
//   },0)
  export default {
    data () {
      return {
        logo: 'https://gw.alicdn.com/tfs/TB1yopEdgoQMeJjy1XaXXcSsFXa-640-302.png',
      }
    }
  }
</script>

<style scoped>
  .wrapper {
    justify-content: center;
    align-items: center;
  }
  .logo {
    width: 424px;
    height: 200px;
  }
  .greeting {
    margin-top: 70px;
    font-size: 50px;
    color: #41B883;
  }
  .message {
    margin: 30px;
    font-size: 32px;
    color: #727272;
  }
</style>
