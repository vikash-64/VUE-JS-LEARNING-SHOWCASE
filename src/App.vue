<template>

<!-- <Card>Hello Card 1</Card>
<br>
<Card>Hello Card 2</Card>
<br>
<Card> <b>Hello Card 3</b></Card> -->

<!-- <slot-comp>
   
</slot-comp>

<slot-comp>
    <h4>Hello from app </h4>
</slot-comp>

<slot-comp>
   
</slot-comp>

<ul v-for="item in items">

   <li>{{ item }}</li>

</ul> -->


<!-- more slot -->

<h1>Parent component</h1>

<!-- header  -->
<MoreSlot>
   <template v-slot:header>
       <h3>This is header slot</h3>
   </template>

<!-- content -->

   <template v-slot:content>
       <h3>This is content slot </h3>
   </template>


<!-- footer goes here -->

   <template v-slot:footer>
       <h3>This is footer slot </h3>
   </template>

   
   
</MoreSlot>




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



export default{

   name:"App",
 
//   adding components here 
   components:{
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

},

//  adding 

   data(){
    return {
      name:'',
      showPopup: false ,
      newItem: '',
      items: ['Buy apples','Make pizza','Mow the lawn']
    }
   },

//  adding methods here  

   methods:{

      addItem(){
        this.items.push(this.newItem),
        this.newItem = '';
      }
   
   }



}

</script>



<!-- style  -->
<style>



</style>