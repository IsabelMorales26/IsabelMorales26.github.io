<template>
    <sui-container text class="down">
        <div class="cardStyle" v-for="item in sectionContent" v-bind:key="item"> 
            <img :src = "require(`../assets/${item.imgDir}`)" class="CardImage"/>
        </div> 
    </sui-container>
</template>
<script>

export default {
    name : 'Section',
    props : {
        sectionContent : Array
    }    
}
</script>
<style scoped>
    .down{
        margin-top: 3rem;
    }
    .question{
        font-size: 2rem;
        font-style: oblique;
    }
    .cardStyle{
        border-style: solid;
        border-width: 1px;
        border-color: grey;
    }
    .CardImage{
        height: 100%;
        width: 100%
    }
</style>