<template>
    <div class="breadcrumb-area bg-gray">
        <div class="container">
            <div class="breadcrumb-content text-center">
                <ul>
                    <li>
                        <router-link to="/" >Home</router-link>
                    </li>
                    <li class="active">Shop </li>
                </ul>
            </div>
        </div>
    </div>

</template>

<script>
    export default {
        name: "Breadcrumb_area"
    }
</script>

<style scoped>

</style>