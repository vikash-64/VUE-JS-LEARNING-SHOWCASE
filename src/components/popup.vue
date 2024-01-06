<template>
    <div>
            <h2>This is PopUp</h2>
            <button @click="$emit('close')" >Close PopUp</button>
    </div>
</template>

<script>
    export default {
        name:'popup',
        emit:['close'],
    }
</script>

