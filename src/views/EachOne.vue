<template>
    <div>
        {{$route.params.id}}

        <button @click="myClick">Back</button>
    </div>
</template>
<script>
import router from "../router/index.js"
export default {
    methods:{
        myClick(){
            router.go(-1)
        }
    }
}
</script>