<template>

    <div class="card">

        <slot name="header">

        </slot>

        <slot name="content">

        </slot>

        <slot name="footer">

        </slot>

    </div>

</template>

<script>

export default{
    name:'Card',


}
</script>


<style scoped>
.card{
  border: 2px solid ;
  height: 100px;
  width: 100px ;  
}
</style>