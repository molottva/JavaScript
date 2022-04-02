<template>
    <div class="modal fade " id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
                    <div class="modal-dialog">
                        <div class="modal-content bg-light border-dark">
                            <div class="modal-header">
                                <h5 class="modal-title" id="exampleModalLabel">{{character.name}} ({{character.nameor}})</h5>
                                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                            </div>
                            <div class="modal-body">
                                <img :src="character.thumbnail" class="img-fluid rounded-start" alt="...">
                                <div>
                                    <h5>Описание:</h5>
                                    <p>{{character.description}}</p>
                                    
                                    <h5>Комиксы:</h5>
                                    <ul>
                                        <li v-for="(comic, i) in character.comics" :key="i">{{comic.name}}</li>
                                    </ul>
                                </div>
                            </div>
                            <div class="modal-footer">
                                <button type="button" class="btn btn-dark" data-bs-dismiss="modal">Закрыть</button>
                            </div>
                        </div>
                    </div>
                </div>
</template>

<script>
    export default {
        name: "AppModal",
        props: ['character'],
    }
</script>

<style scoped>

</style>
