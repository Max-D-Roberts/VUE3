<template>
    <div>
        <div class="person">
            <h2>name: {{mike.name }}</h2>
            <h2> age: {{mike.age }}</h2>
        </div>
    </div>
</template>
<script lang="ts" setup>
import {reactive, ref,toRefs} from 'vue';
let {name,age}=reactive({name:'max',age:25})
let mike={name:'max',age:25}
console.log('person=>',name);
console.log('mike=>',age);

</script>
<style scoped>
.person {
    font-size: 20px;
}
</style>