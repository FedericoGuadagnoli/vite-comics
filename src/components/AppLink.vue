<script>
export default {
    name: 'AppLogo',
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    },

    methods: {
        setCurrent(link) {
            this.links.forEach(link => link.current = false);
            link.current = true;
        }
    }
};
</script>

<template>
    <ul>
        <li v-for="link in links" :class="{ 'active': link.current }" @:mouseover="setCurrent(link)"
            @:mouseout="setCurrent(link)">
            <a :href="link.url">{{ link.text }}</a>
        </li>
    </ul>

</template>

<style scoped>
ul {
    display: flex;
    align-items: center;
}

ul li {
    list-style-type: none;
    margin-right: 2rem;
    font-size: 1.25rem;
    display: flex;
    align-items: center;
    cursor: pointer;
}

ul,
li {
    height: 100%;
}

ul li a {
    color: black;
}

.active {
    border-bottom: 5px solid dodgerblue;
    transform: translateY(3px);
}
</style>