<script>
export default {
    name: 'AppContent',
}
</script>

<template>
    <div id="content">
        <h2>content</h2>
    </div>
</template>

<style lang="scss">
@use '../styles/variables.scss' as *;

#content {
    background-color: black;
    height: 100px;

    h2 {
        padding: 50px 80px;
        color: white;
        display: flex;
        justify-content: flex-start;
    }
}
</style>