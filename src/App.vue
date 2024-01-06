<template>

<h4>App class</h4>



<Button @click="activeTab = 'TabA'" >TabA</Button>
<button @click="activeTab = 'TabB'" >TabB</button>
<button @click="activeTab = 'TabC'" >TabC</button>

<KeepAlive>
<component :is="activeTab"/>
</KeepAlive>

<!-- <TabA v-if="activeTab === 'TabA'" />
<TabB v-if="activeTab === 'TabB'" />
<TabC v-if="activeTab === 'TabC'" /> -->








</template>

<!-- script  -->

<script>

import greet from './components/greet.vue';
import Article from './components/Article.vue';
import popup from './components/popup.vue';
import FoodItem from './components/FoodItem.vue';
import Emit from './components/Emit.vue';
import TodoItem from './components/TodoItem.vue';
import Input from './components/Input.vue';
import Card from './components/Card.vue';
import SlotComp from './components/SlotComp.vue';
import MoreSlot from './components/MoreSlot.vue';
import PropSlot from './components/PropSlot.vue';
import ChildStyles from './components/ChildStyles.vue';
import TabA  from './components/TabA.vue';
import TabB  from './components/TabB.vue';
import TabC  from './components/TabC.vue';



export default {

   name: "App",

   //   adding components here 
   components: {
      greet,
      Article,
      popup,
      FoodItem,
      Emit,
      TodoItem,
      Input,
      Card,
      SlotComp,
      MoreSlot,
      PropSlot,
      ChildStyles,
      TabA,
      TabB,
      TabC,



   },

   //  adding data 

   data() {
      return {

         activeTab: 'TabA'

      }
   }

}

</script>



<!-- style  -->
<style>

#app{

   background-color: antiquewhite;
   text-align: center;

}

h4{
    color: red;
    text-decoration: solid;
}

button {
  background-color: #62eeee; 
  border: solid black;
  border-style: double;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 5px;
  border-radius: 12px ;

}
button:hover {background-color: #084c94}




</style>