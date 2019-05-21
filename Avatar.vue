<template>
    <div>
        <h1 v-if="msg">{{msg}}</h1>
        <h1>Avatars:</h1>

        <div :key="avatar.length" v-for="avatar in data">
            <div>
                <h3>
                    {{avatar.title}}
                </h3>
                <i :style="{ 'background': 'url(./assets/' + avatar.img + ')' }"></i>
            </div>
        </div>


    </div>
</template>

<script>
export default {
    name: 'Avatars',
    props: [ 'msg', 'data']
}
</script>

<style>

</style>
