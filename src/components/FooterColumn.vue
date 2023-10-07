<script setup>
const props = defineProps({
    data: {
        type: Object,
        required: true
    }
})

</script>

<template>
    <div class="footer-column">
        <h3>{{ data.title }}</h3>
        <ul>
            <li v-for="link in data.links" :key="link.text">
                <a :href="link.href">{{ link.text }}</a>
            </li>
        </ul>
        <template v-if="data.subcolumn">
            <h4>{{ data.subcolumn.title }}</h4>
            <ul>
                <li v-for="link in data.subcolumn.links" :key="link.text">
                    <a :href="link.href">{{ link.text }}</a>
                </li>
            </ul>
        </template>
    </div>
</template>

<style scoped>
.footer-column {
    margin: 0 20px;
}

h3 {
    color: #fff;
    font-weight: 600;
    font-size: 24px;
    margin-bottom: 10px;
}

h4 {
    color: #fff;
    font-weight: 600;
    font-size: 18px;
    margin-top: 20px;
}

ul {
    list-style: none;
    padding: 0;
}

a {
    color: #fff;
    text-decoration: none;
}
</style>