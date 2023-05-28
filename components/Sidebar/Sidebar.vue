<template lang="">


    <div class="w-[522px]">
        <div class="mt-[92px] w-[100%] text-[24px] font-semibold">

            <p>Latest articles</p>
        </div>
        <div class="p-[20px] bg-white mt-[24px] rounded-[18px]">
            <ul v-for="(el,ind) in latestArticles" class="px-[20px]">
                <li class="list-disc text-[#AAAAAA] mb-[16px]">{{el}}</li>
            </ul>
        </div>

        <div class="my-[30px] w-[100%] text-[24px] font-semibold">
            <p>Tags</p>
        </div>
        <div v-for="(el,ind) in tags" class="flex">
            <span class=" m-[10px] bg-white rounded-[100px] inline px-[10px] py-[10px] text-[#AAAAAA]">{{el.tag}} ({{el.sum}})</span>
        </div>
    </div>

</template>
<script setup>
let latestArticles = [
    "Ingliz tilidagi so'zlarni eslab qolishing 11 ta samarali usuli",
    "Ingliz tilini samarali o'rganish uchun 7 ta maslahat",
    "O‘zbek tilining asosiy imlo qoidalari",
    "Upwork'da ish boshlash",
    "Most Confused Words in English",
    "Most Confused Words in English"
]

let tags = [
    {
        tag: 'English',
        sum: 2
    },
    {
        tag: 'Freelancer',
        sum: 5
    },
    {
        tag: 'Vocabulary',
        sum: 5
    },
    {
        tag: 'Uzbek Grammer',
        sum: 2
    },
    {
        tag: 'English Grammer',
        sum: 2
    },
    {
        tag: 'Imlo',
        sum: 2
    },
]
</script>
<style lang="">
    
</style>