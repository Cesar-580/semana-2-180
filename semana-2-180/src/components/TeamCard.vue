<template>

                                <div class="card text-white bg-dark">
                                    <div class="d-flex justify-content-center p-2">
                                        <img v-bind:src="member.imagen" alt="FotoDelEquipo" style="width:160px;height:150px;padding-bottom: 5px">
                                </div>
                                <div class="card-body" style="height:290px;padding-bottom: 5px">
                                    <p class="card-text" style="height:40px"><center><span>  Team member:  {{member.codigo}} </span>
                                        <span>{{member.rol}}</span></center>
                                    </p>
                                    <h5 class="card-title" style="height:50px"><center>{{ member.nombre}}</center></h5>
                                    <p class="card-text" style="height:140px"><center>{{member.descripcion}}</center></p>
                                    
                                    </div>
                                    <div class="card-footer">
                                        <small class="text-muted">Last updated 3 mins
                                            ago</small>
                                        </div>
                                    </div>

</template>

<script>
    export default {
        name: 'TeamCard',
        props: ['member']

        // props: {
        //     'member' :Object
        // }
    }
</script>

<style scoped>

</style>
