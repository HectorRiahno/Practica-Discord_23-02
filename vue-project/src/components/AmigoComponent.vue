<script setup>
const props=defineProps({
    amigo:{
        type:String,
        default:''
    },
    index:{
        type:Number
    }
})
// const emit=defineEmits(['marcos'])
// function marcos(i){
//     emit('marcos',i)
// }
</script>
<template>
    <div v-for="(obj,i) in props[indice].mensaje1" :key="i" >
        <div v-if="props[indice].mensaje1[i]!=null" class="relative bg-black/50 text-white/50 mt-6 p-2 rounded-md border border-white/30">
          <p class=""> {{ props[indice].mensaje1[i] }}</p>
          <p class="text-end font-extralight text-xs mt-2">24/12/2023 12:00am</p>
        </div>
      </div>
</template>