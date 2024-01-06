<template>
  <div>
    <h2>{{ foodName }}</h2>
    <p>{{ foodDesc }}</p>
    <button @click="toogleFav">Click here to toogle</button>
  </div>
 
</template>
  
<script>
export default {

  // adding data here  

  data() {
    return {
      name: 'Apples',
      message: 'I like '
    }
  },

  // adding props here 
  props: {

    foodName: {
      type: String

    },
    foodDesc: {
      type: String,
      validator: function (value) {

        if (20 < value.length && value.length < 50) {
          return true;
        }
        else {
          return false;
        }
      }
    }

  },

  //  adding methods here  

  methods:{
     toogleFav(){
      this.$emit('toogle-fav' , "Hello aagya mai");
     }
  }


};
</script>
  
<style></style>