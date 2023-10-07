<script setup>
</script>

<template>
    <header>
        <h1>How can we help?</h1>
        <div>
            <input type="search" placeholder="Search" class="search-input">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                style="fill: rgba(0, 0, 0, 1);transform: ;msFilter:;" class="right-arrow">
                <path d="m11.293 17.293 1.414 1.414L19.414 12l-6.707-6.707-1.414 1.414L15.586 11H6v2h9.586z"></path>
            </svg>
        </div>
    </header>
</template>

<style scoped>
header {
    height: 400px;
    width: 100vw;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #dadbf1;
}

header h1 {
    font-size: 72px;
    color: #000;
    margin-bottom: 20px;
}

.search-input {
    width: 700px;
    height: 64px;
    font-size: larger;
    border-radius: 4px;
    border: 2px solid #000;
    padding: 16px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
}

.search-input:hover,
.search-input:focus {
    border: 2px solid #4c5fd5;
}

.right-arrow {
    margin-left: -40px;
    top: 4px;
}
</style>
