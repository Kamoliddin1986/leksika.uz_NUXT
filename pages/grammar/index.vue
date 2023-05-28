<template lang="">

    <div class="w-full grid place-items-center">
        <div class="w-[80%] grid place-items-center my-[60px]">
            <h1 class="text-[24px] font-semibold">TABLE OF CONTENTS</h1>
            <div v-for="(el,ind) in gram" class="w-[80%] bg-[#CBFDF4] h-[98px] flex rounded-[32px] my-[16px] items-center justify-between">
                <div class="flex items-center">

                    <div class="w-[50px] h-[50px] rounded-full bg-[#01756C] ml-[32px] mr-[16px] flex justify-center items-center text-white text-[20px]">0{{el.id}}</div>  
                    <h1 class="text-[18px] font-normal">{{el.title}}</h1>
                </div>
                <div class="w-[50px] h-[50px] rounded-full bg-white mr-[22px]  flex justify-center items-center text-white">
                        <Icon name="material-symbols:add-rounded" class="font-extrabold text-[24px]" color="#01756C" />

                    </div>  
                
            </div>
        </div>
    </div>
</template>
<script setup>


let gram = [
    {
        id: 1,
        title: 'Introduction',        
    },
    {
        id: 2,
        title: 'Present Simple',        
    },
    {
        id: 3,
        title: 'Present Contunues',        
    },
    {
        id: 4,
        title: 'Post Simple',        
    },
    {
        id: 5,
        title: 'Infinity, Gerund',        
    }
]
</script>
<style lang="">
    
</style>