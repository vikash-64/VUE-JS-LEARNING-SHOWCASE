<template>
        <div>
        <h1>{{ articleName }}</h1>
        <p v-bind="$attrs">{{ articleNum }}</p>
        <p>{{ articlePublish ? 'yes' : 'No' }}</p>
        </div>
</template>

<script>
    export default {

        name:'Article',
        props:{

            articleName:{

                type:String,
                required: true , 
            
            },

            articleNum:{

                type:Number,
                default: 0 

            },
            articlePublish:{

                type:Boolean


            }
        },
        inheritAttrs:false 
    }


</script>

