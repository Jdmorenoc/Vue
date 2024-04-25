<script setup>
    import { ref } from 'vue'

    let count = ref(0);

    function addvalue() {
        count.value++;
        console.log(count);
    }
</script>


<template>
    <div @click="addvalue();" class="bg-blue-500 text-white py-2 px-4 rounded inline-block hover:cursor-pointer hover:bg-blue-600 transition-colors">
        ¡Golepame! {{ count }}
    </div>
</template>