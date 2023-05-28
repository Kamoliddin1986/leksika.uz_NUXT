
<template lang="">
    <div class="columns-2 px-[80px] flex justify-between gap-[20px] bg-[#F1F4F6]">
        <div class="w-[120%]">
                        
                        <input type="search" name="" id="" placeholder="search article here" class=" p-[15px] mt-[60px] w-[100%] h-[64px] mb-[20px] rounded-[18px]">
            <div v-for="(el,ind) in article" :key="ind" class="columns-2 h-[265px] bg-white rounded-[18px] mb-[20px] ">
                <div class="w-[70%]  m-[20px] h-[225px]">
                    <img :src="el.img" class="w-[100%] h-[100%]  rounded-[18px]" alt="">
                </div>
                <div class="w-[100%] h-[225px]  mr-[20px] mt-[20px]">
                    <div>
                        <Icon name="material-symbols:calendar-month-outline-rounded" color="white" />
                        <span>{{el.last_read}} month ago</span>

                        <Icon name="ph:book-open" color="white" />
                        <span>number of reads: {{el.total_reads}}</span>
                    </div>
                    <h1>{{el.title}}</h1>
                    <p class="text-[16px] text-left">{{el.text}}</p>
                </div>
            </div>
        </div>
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

        
    </div>
</template>
<script setup>

let article = [
    {
        img: 'https://picsum.photos/id/255/200/300',
        title: 'Ingliz tilidagi sozlarni eslab qolishing 11 ta samarali usuli',
        text: "Chet tilini o’rganishda so’z boyligini doimiy ravishda boyitib borish, ya’ni ko’proq yangi so’zlarni yod olish, juda muhimdir. Biroq, hamma ham bu ishni uddalay olmaydi. So’z boyligini oshirish",
        last_read: 1,
        total_reads: 2
    },
    {
        img: 'https://picsum.photos/id/255/200/300',
        title: 'Ingliz tilidagi sozlarni eslab qolishing 11 ta samarali usuli',
        text: "Chet tilini o’rganishda so’z boyligini doimiy ravishda boyitib borish, ya’ni ko’proq yangi so’zlarni yod olish, juda muhimdir. Biroq, hamma ham bu ishni uddalay olmaydi. So’z boyligini oshirish",
        last_read: 1,
        total_reads: 52
    },
    {
        img: 'https://picsum.photos/id/255/200/300',
        title: 'Ingliz tilidagi sozlarni eslab qolishing 11 ta samarali usuli',
        text: "Chet tilini o’rganishda so’z boyligini doimiy ravishda boyitib borish, ya’ni ko’proq yangi so’zlarni yod olish, juda muhimdir. Biroq, hamma ham bu ishni uddalay olmaydi. So’z boyligini oshirish",
        last_read: 1,
        total_reads: 52
    },
    {
        img: 'https://picsum.photos/id/255/200/300',
        title: 'Ingliz tilidagi sozlarni eslab qolishing 11 ta samarali usuli',
        text: "Chet tilini o’rganishda so’z boyligini doimiy ravishda boyitib borish, ya’ni ko’proq yangi so’zlarni yod olish, juda muhimdir. Biroq, hamma ham bu ishni uddalay olmaydi. So’z boyligini oshirish",
        last_read: 1,
        total_reads: 52
    },
    {
        img: 'https://picsum.photos/id/255/200/300',
        title: 'Ingliz tilidagi sozlarni eslab qolishing 11 ta samarali usuli',
        text: "Chet tilini o’rganishda so’z boyligini doimiy ravishda boyitib borish, ya’ni ko’proq yangi so’zlarni yod olish, juda muhimdir. Biroq, hamma ham bu ishni uddalay olmaydi. So’z boyligini oshirish",
        last_read: 1,
        total_reads: 52
    },
    {
        img: 'https://picsum.photos/id/255/200/300',
        title: 'Ingliz tilidagi sozlarni eslab qolishing 11 ta samarali usuli',
        text: "Chet tilini o’rganishda so’z boyligini doimiy ravishda boyitib borish, ya’ni ko’proq yangi so’zlarni yod olish, juda muhimdir. Biroq, hamma ham bu ishni uddalay olmaydi. So’z boyligini oshirish",
        last_read: 1,
        total_reads: 52
    },
]

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