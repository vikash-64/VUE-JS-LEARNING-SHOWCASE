<template>

<h3 v-for="name in names"  :key='names.firstName'>

    <slot :firstName="name.firstName" :lastName="name.lastName"></slot>

    
</h3>

</template>


<script>


export default {

    data() {
        return {
            names: [
                {
                    firstName: 'John',
                    lastName: 'Doe',
                },


                {
                    firstName: 'Alice',
                    lastName: 'Smith',
                },


                {
                    firstName: 'Bob',
                    lastName: 'Johnson',
                },
            ]
        }
    }

}


</script>

<style></style>


<!-- this below code is for the app.vue in templement -->

<!-- 

       <PropSlot>

      <template v-slot:default="SlotProps">

         {{ SlotProps.firstName }} {{ SlotProps.lastName }}

      </template>
   </PropSlot>

   <PropSlot>
      <template v-slot:default="SlotProps">

         {{ SlotProps.firstName }}

      </template>

   </PropSlot>
</template>

 -->