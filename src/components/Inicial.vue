<template>
    <div class="bg-gray-800 flex text-white max-h-screen h-screen ">
        <div class=" w-64">
            <span class="font-semibold px-6 pt-3 ">skateboard</span>

            <nav class="p-6">
                <h3 class="opacity-50 font-bold uppercase">Menu</h3>

                <div class="space-y-3">
                    <ItemMenu :icon="HomeIcon">MiniMenu1</ItemMenu>
                    <ItemMenu :icon="TrendUpIcon">Opção1</ItemMenu> 
                    <ItemMenu :icon="TrendUpIcon">Opção2</ItemMenu> 
                    <ItemMenu :icon="TrendUpIcon">Opção3</ItemMenu> 
                    <ItemMenu :icon="TrendUpIcon">Opção4</ItemMenu> 
                </div>
                <div class="space-y-3 pt-10">
                    <ItemMenu :icon="HomeIcon">MiniMenu2</ItemMenu>
                    <ItemMenu :icon="TrendUpIcon">Opção1</ItemMenu> 
                    <ItemMenu :icon="TrendUpIcon">Opção2</ItemMenu> 
                    <ItemMenu :icon="TrendUpIcon">Opção3</ItemMenu> 
                    <ItemMenu :icon="TrendUpIcon">Opção4</ItemMenu> 
                </div>
                
            </nav>
        </div>

        <div class="p-5 flex-1 h-screen overflow-y-auto">
            <header class="flex items-center justify-between">
                <InputSearch class="w-96"/>
                <div class="flex">
                    
                    <div class="flex items-center space-x-3">
                        <Avatar class="w-5 h-5" />

                        <span>Umdyne</span>
                        <ChevronDownIcon class="w-4 h-4"/>
                    </div>

                    <Notification />    
                    <BellIcon class="opacity-50 hover:opacity-100 cursor-pointer transition duration-500" />
                    
                </div>
            </header>   
            <h1 class="font-bold text-4xl mt-6 mb-4">Discover</h1>  
            <div class="grid gap-4 grid-cols-12">
                <div class="col-span-8 h-96 rounded-3xl overflow-hidden relative"> 
                    <div class="flex w-full h-full"> 
                        <img src="https://via.placeholder.com/2000x1400" class="w-full object-cover">
                        
                    </div>
                    <div class="z-10 absolute top-0 p-5 w-full h-full bottom-0 "> 
                       <h3 class="text-2xl max-w-xs">How to do basic jumping and how to landing safely</h3>  
                       <div class="absolute right-6 bottom-6 px-2 py-1 rounded-lg bg-gray-700 text-white"> 
                            7 Minutes
                       </div>
                    </div>
                     
                </div> 

                <div class="col-span-4 h-96 rounded-3xl overflow-hidden relative"> 
                    <div class="flex w-full h-full"> 
                        <img src="https://via.placeholder.com/2000x1400" class="w-full object-cover">
                        
                    </div>
                    <div class="z-10 absolute top-0 p-5 w-full h-full bottom-0 "> 
                       <h3 class="text-2xl max-w-xs">How to dont basic jumping and how to landing safely</h3>  
                       <div class="absolute right-6 bottom-6 px-2 py-1 rounded-lg bg-gray-700 text-white"> 
                            7 Minutes
                       </div>
                    </div>
                     
                </div>
                
            </div>  
            <h1 class="font-semibold text-2xl mt-6 mb-4">MostWatched</h1> 
            <div class="grid grid-cols-4 gap-4">
                <ItemCard v-for="n of 4"/> 

            </div>
        </div>

    </div>
</template>

<script lang="ts" setup>

    import ItemMenu from './navs/ItemMenu.vue';
    import HomeIcon from './icons/HomeIcon.vue';
    import TrendUpIcon from './icons/TrendUpIcon.vue';
    import InputSearch from './inputs/InputSearch.vue';
    import Avatar from './Avatar.vue'
    import BellIcon from './icons/BellIcon.vue'
    import ItemCard from './ItemCard.vue'

 
</script>
