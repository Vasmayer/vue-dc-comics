<template>
    <main>
        <h1>Content goes here</h1>
    </main>
</template>

<script>
export default {
    name:'Content'
}
</script>

<style lang="scss" scoped>

$color_content:#1C1C1C;

main
{
    height: 200px;
    background-color: $color_content;
    display: flex;
    align-items: center;
    justify-content: space-around;

    h1{
        color:white;
    }
}
</style>