<template>
<h3>Child Components</h3>

<!--  header goes here -->
<div class="header">
    <slot name="header">

    </slot>
</div>
<!-- content goes here -->
<div class="content">
    <slot name="content">

    </slot>
</div>

<!-- footer goes here -->

<div class="footer">
    <slot name="footer">

    </slot>
</div>

<!-- default slot -->
<div class="default">
    <slot></slot>
</div>


</template>

<!-- script goes here -->

<script>

export default{

}

</script>

<!-- style yha aaega  -->
<style>

</style>