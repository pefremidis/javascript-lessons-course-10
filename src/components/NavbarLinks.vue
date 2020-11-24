<template>
    <ul class="flex">
        <NavbarLink v-for="(link, index) in links" :key="index">
            <template v-if="link.to">
                <router-link :to="link.to">{{ link.name }}</router-link>
            </template>

            <template v-else>
                {{ link.name }}
            </template>
        </NavbarLink>
    </ul>
</template>

<script>
    import NavbarLink from "./NavbarLink";

    export default {
        name: "NavbarLinks",

        data() {
            return {
                links: [
                    {
                        name: 'Αρχική',
                        to: '/'
                    },
                    {
                        name: 'Axia Broker',
                        to: ''
                    },
                    {
                        name: 'Ενέργεια',
                        to: ''
                    },
                    {
                        name: 'Ασφάλεια',
                        to: ''
                    },
                    {
                        name: 'Χρηματιστήριο',
                        to: ''
                    },
                    {
                        name: 'Επικοινωνία',
                        to: '/about'
                    }
                ]
            }
        },

        components: {
            NavbarLink
        }
    }
</script>
