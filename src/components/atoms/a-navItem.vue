<template>
    <li >
        <a href="#"
           class = "no-underline text-inherit" 
        >{{text}}</a>
    </li>
</template>

<script>
export default {
    name: "navItem",
    props: {
        text: {
            type: String,
        }
    },
}
</script>

<style>

</style>