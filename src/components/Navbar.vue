<template>
    <div class="flex justify-between h-20 items-center px-8 shadow-xl">
        <div>
            <img class="h-10" src="../assets/logo.png"/>
        </div>

        <div>
            <NavbarLinks/>
        </div>
    </div>
</template>

<script>
    import NavbarLinks from "./NavbarLinks";

    export default {
        name: "Navbar",

        components: {
            NavbarLinks
        }
    }
</script>
