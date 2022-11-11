<script>
export default {
name: 'Comic',
props:{
    image: String,
    title: String
},
}
</script>

<template>
    <div class="col">
        <div class="comic">
            <img :src="thumb" alt="">
            <h4>{{ series }}</h4>
        </div>
    </div>
</template>