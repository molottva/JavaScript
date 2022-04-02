<template>
    <nav class="navbar navbar-dark bg-dark">
        <div class="container-fluid">
            <a class="navbar-brand">Marvel</a>
            <form class="d-flex">
                <input class="form-control me-2" type="search" placeholder="Введите имя..." aria-label="Search">
                <button class="btn btn-dark btn-outline-light text-white" type="submit">Поиск</button>
            </form>
        </div>
    </nav>
</template>

<script>
    export default {
        name: "AppHeader",
        data() {
            return {
            }
        },
    }
</script>

<style scoped>

</style>
