<template>
<div class="link">
    <h3>Lista de links requeridos</h3>
    <ul>
        <li v-for="item in vals" v-bind:key="item">
            <a :href= item.link >
                {{item.desc}}
            </a>
        </li>    
    </ul>
    
   
</div>
    
</template>
<script>
export default {
    name: 'Links',
    props: {
        vals: Array
    }    
}
</script>
<style scoped>
    .link{
        margin-top: 5%;
    }
</style>