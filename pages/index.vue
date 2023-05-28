<template lang="">
    <div class=" flex flex-col items-center bg-[#F1F4F6]">

        <div class="mt-[60px] w-[874px] h-[74px] bg-white rounded-[100px]">
            
            <button class="w-[174px] h-[64px] rounded-[100px] bg-[#01756C] m-[5px]">ENG <Icon name="nimbus:arrows-horizontal" color="white" />UZB</button>
            <input v-model="word" @keydown.enter="find" type="search">
        </div>
        <div  v-if="!getData?.data" class="w-[606px] h-[141px] mt-[144px]">
            <p class="text-[24px] text-center">Search any words, and we found this word defination, translation and etc.</p>

        </div>
        <div  v-else-if="!getData.data.value" class="w-[606px] h-[141px] mt-[144px] flex justify-center">
            <img src="../assets/icons/sheksper 1.svg" alt=""> <img src="../assets/icons/Group 22.svg" alt="">

        </div>

        <div  v-else class="w-[846px] rounded-[18px] h-[225px] px-[18px] py-[32px] mt-[40px] bg-white">
            <h1 class="text-[32px] ">{{getData.data.value[0].word}}</h1>
            
            <div class="flex gap-[10px] items-center">
                <Icon name="mdi:volume-high" color="black" @click="playSound" />
                <h3>{{getData.data.value[0].phonetics[1].text}}</h3>
            </div>
        </div>
    </div>
</template>
<script setup>
let word = ref('')
let getData 
const find = async() => {

    getData = await useFetch(`https://api.dictionaryapi.dev/api/v2/entries/en/${word.value}`)
    console.log(data);
}

const playSound = () => {
    const sound = new Audio(getData.data.value[0].phonetics[0].audio)
    sound.play()
}

</script>
<style lang="">
    
</style>