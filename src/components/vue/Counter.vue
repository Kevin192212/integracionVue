<script setup>

import { ref } from 'vue'
    let count = ref(0);

    function addvalues(){
        count.value++;
        console.log(count)
    }
</script>

<template>
    <div @click="addvalues()" class="bg-blue-500 text-white py-2 px-4 rounded inline-block hover:cursor-pointer hover:bg-blue-600 transition-colors">
        ¡Touch! {{ count }}
    </div>
</template>