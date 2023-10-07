<script setup>
import { reactive } from 'vue';
import FooterColumn from './FooterColumn.vue';
import TheCopyright from './TheCopyright.vue';

const footerColumns = reactive({
    column1: {
        title: 'Abstract',
        links: [
            { text: 'Start Trial', href: '#' },
            { text: 'Pricing', href: '#' },
            { text: 'Download', href: '#' },
        ]
    },
    column2: {
        title: 'Resources',
        links: [
            { text: 'Blog', href: '#' },
            { text: 'Help Center', href: '#' },
            { text: 'Release Notes', href: '#' },
            { text: 'Status', href: '#' },
        ]
    },
    column3: {
        title: 'Community',
        links: [
            { text: 'Twitter', href: '#' },
            { text: 'LinkedIn', href: '#' },
            { text: 'Facebook', href: '#' },
            { text: 'Dribble', href: '#' },
            { text: 'Podcast', href: '#' },
        ]
    },
    column4: {
        title: 'Company',
        links: [
            { text: 'About Us', href: '#' },
            { text: 'Careers', href: '#' },
            { text: 'Legal', href: '#' },
        ],
        subcolumn: {
            title: 'Contact Us',
            links: [
                { text: 'info@abstact.com', href: '#' },
            ]
        }
    },
})

</script>

<template>
    <footer>
        <FooterColumn v-for="column in footerColumns" :data="column" />
        <TheCopyright />
    </footer>
</template>

<style>
footer {
    position: relative;
    height: 400px;
    background-color: #000;
    display: flex;
    padding: 42px 64px 100px;
}
</style>