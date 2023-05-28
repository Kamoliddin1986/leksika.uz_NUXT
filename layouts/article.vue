<template lang="">
    <Header/>
    <main class="min-h-screen bg-[#F1F4F6]">

        <div class="columns-2 px-[80px] flex justify-between gap-[20px] bg-[#F1F4F6]">
            
                <slot/>
            
            

                <Sidebar/>
            
            
            
        </div>
    </main>
    <Footer/>
</template>
<script setup>

</script>
<style lang="">
    
</style>