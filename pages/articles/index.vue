
<template lang="">

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
                    <NuxtLink :to="`/articles/el.${el.id}`" class="text-[24px] ">{{el.title}}</NuxtLink>
                    <p class="text-[16px] text-left">{{el.text}}</p>
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

definePageMeta({
    layout: 'article'
})



</script>
<style lang="">
    
</style>