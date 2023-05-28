<template lang="">

        <div class=" flex w-full pt-[60px] mb-[80px] justify-center">
            <p class="w-[846px]  h-[135px] text-[18px] text-center" >Remember the days when you couldn’t find the proper translation of an English word to the Uzbek language? I also know those feelings when you run against the lack of general use dictionaries - not to mention the specialized ones, a total absence of online resources in Uzbek, a pre-requisite of knowing the Russian language in order to apply indirect translation (EN RU UZ and vice versa).</p>
        </div>
        
        <div class="w-full flex justify-center">
            <div class="w-[80%] h-[0px] border border-[#DDDDDD]"></div>
        </div>

        <div v-for="(el,ind) in info" :key="ind" class="w-full flex justify-between px-[80px] my-[60px]">
            <div class="w-[30%] align-left">
                <h1 class="text-[#01756C] text-[24px] font-semibold">{{el.title}}</h1>
            </div>
            <div class="w-[60%] text-[16px]">
                <p >{{el.text}}</p>
               
            </div>
        </div>

        <div class="w-full flex justify-center">
            <div class="w-[80%] h-[0px] border border-[#DDDDDD]"></div>
        </div>

        <div  class="w-full flex justify-between px-[80px] mt-[60px] pb-[60px]">
            <div class="w-[30%] align-left">
                <h1 class="text-[#01756C] text-[24px] font-semibold">OUR TEAME</h1>
            </div>
            <div v-for="(el,ind) in ourTeame " :key="ind" class="flex">

                <div  class=" card w-[414px] h-[560px] bg-white rounded-[10px]">
                    <img :src="el.img" alt="" class="w-full h-[427px] rounded-[10px]">
                    <h3 class="text-[24px] font-normal mt-[20px] mb-[10px] text-center">{{el.name}}</h3>
                    <div class="w-full flex justify-center">
                        <div class="w-[130px] h-[0px] border border-[#01756C] "></div>
                    </div>
                    <h5 class="text-center">{{el.position}}</h5>
                </div>
            </div>
        </div>

</template>
<script setup>

let info = [
    {
        id: 1,
        title: 'Book edition',
        text: "To reverse the situation, it was decided to compile a large English-Uzbek-English dictionary and the work started back in 2003. 2 years later, the first edition of the bilingual dictionary was published in G’afur G’ulom publishing house; it is still available for sale online. Much attention was directed to the Uzbek-English part; even now, it is the most comprehensive and complete UZ-EN dictionary A mobile app for Android devices was launched based on the dictionary with ma jor update of the lexical database."
    },
    {
        id: 2,
        title: 'Website dictionary',
        text: " However, we still desperately needed a high-quality online dictionary for English-Uzbek language pair that could cover both everyday and area-specific vocabulary. In September 2022, on the date of 31th anniversary of Independence of Uzbekistan, Leksika.uz was successfully launched Leksika.uz has mainly been designed to give English learners of any level the help they need to read, speak and write English more effectively. It is also intended to assist translators and localizers by providing useful tips and rules of thumb; these can be found in Localization section."
    },
    {
        id: 3,
        title: 'Prospects',
        text: 
            "Russian-Uzbek-Russian dictionary section with largest database on the web content for easier learning of English, including grammar, writing tips, learning new words;useful tips and motivational articles for freelancers articles for localizers to Uzbek language, including intricacies of Uzbek grammarand much more."
        
    },
]

let ourTeame = [
    {
        name: 'Ahnan Hunal',
        position: "Founder and content manager",
        img: 'https://picsum.photos/id/10/200/300'
    },
    {
        name: 'Asnan Akbar',
        position: "Full-Stack (MERN) Developer",
        img: 'https://picsum.photos/id/11/200/300'
    },
]
</script>
<style lang="">
    
</style>