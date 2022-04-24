<template>
    <header class="header">
        <a href="" class="toggle">
            <i class="fa fa-lg" :class="icon"></i>
            <h1 class="title"> {{title}}</h1>
            <p>teste</p>
        </a>
    </header>
</template>


<script>
export default {
    name: 'MyHeader',
    props: {
        title: String,
        hideTogle: Boolean
    },
    computed: {
        icon() {
            return "fa-angle-left"
        }
    }
}
</script>


<style>
    .header {
        grid-area: header;
        background: linear-gradient(to right, #1e469a, #49a7c1);

        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>