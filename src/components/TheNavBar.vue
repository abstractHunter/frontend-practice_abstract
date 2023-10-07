<script setup>

</script>
<template>
    <nav>
        <div class="brand">
            <a href="/" class="brand-name">Abstract</a>
            |
            <a href="/">Help Center</a>
        </div>
        <div class="links">
            <a href="/" class="button button-outlined">Submit a request</a>
            <a href="/" class="button button-plain">Sign in</a>
        </div>
    </nav>
</template>

<style scoped>
nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 24px 64px;
    background-color: #000;
    color: #fff;
    font-size: x-large;
}

a {
    text-decoration: none;
    color: #fff;
}

.button {
    margin: 0 12px;
    padding: 8px 20px;
    border-radius: 8px;
}

.button-outlined {
    border: 2px solid #fff;
    background-color: #1a1a1a;
}

.button-plain {
    background-color: #4C5FD5;
}
</style>    