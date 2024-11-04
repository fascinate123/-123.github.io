<template>
  
  <input type="text" v-model.lazy="message">
  <button @click="ght">按钮</button>
  <p>{{ message }}</p>
  <video v-if="message=='蔡徐坤'" src="./抖音2024114-293794.mp3" controls autoplay></video>
  <video v-if="message=='雷军'" src="./抖音2024114-941774.mp3" controls autoplay></video>
  <video v-if="message=='薛之谦'" src="./抖音2024114-769974.mp3" controls autoplay></video>

</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return {
      message:""
    }
  }
  ,methods:{
    ght(){
      if(this.message=="薛之谦"){
        console.log("薛之谦");
        
      }
      else if(this.message=="雷军")
      {
        console.log("雷军");
        
      }
    }
  }

}
</script>

