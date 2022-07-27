<template>
    <div class="bg-gray-800 flex text-white max-h-screen h-screen p-10">
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

        <div class="flex-1 ">
            <header class="flex items-center justify-between">
                <InputSearch />
                <div>
                    

                    <div class="flex items-center space-x-3">
                        <Avatar class="w-5 h-5" />

                        <span>Umdyne</span>
                        <ChevronDownIcon class="w-4 h-4"/>
                    </div>

                    <Notification />    
                </div>
                
            </header>
        </div>
    </div>
</template>

<script lang="ts" setup>

    import ItemMenu from './navs/ItemMenu.vue';
    import HomeIcon from './icons/HomeIcon.vue';
    import TrendUpIcon from './icons/TrendUpIcon.vue';
    import InputSearch from './inputs/InputSearch.vue';
    import Avatar from './Avatar.vue'
</script>
