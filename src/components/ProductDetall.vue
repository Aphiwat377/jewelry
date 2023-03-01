<template>
    <li>
        {{ name }}
    </li>
</template>

<script>
    export default{
        name:"ProductDetall",
        props:{
            id:{
                type:Number
            },
            name:{
                type:String,
                required:true
            },
            detall:{
                type:String,
            },
            type:{
                type:String,
                required:true
            },
            price:{
                type:Number,
                required:true
            },
            picture:{
                type:Array,
                required:true
            },
            color:{
                type:String,
                required:true
            },
            showDetall:{
                type:Boolean
            }

        }
    }
</script>