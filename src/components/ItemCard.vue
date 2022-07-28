<template>
    <div class="bg-gray-900 opacity-90 rounded-3xl overflow-hidden">
        <div class="header"> 
            <div class="h-20 flex w-full"> 
                <img src="https://via.placeholder.com/800x600" class="object-cover w-full h-full">
            </div>
        </div>
   

        <div class="body relative p-2"> 
            <Avatar class="h-10 w-10 rounded-full overflow-hidden absolute right-2 -top-6"/>
            <h5 class="text-xs opacity-50 mb-2">Andy Wood 
                <div class="w-2 h-2 inline-block ml-2 rounded-full bg-gray-300"></div></h5>
            <h4>How to ride skate only skate</h4>
            <div class="text-xs flex items-center space-x-2 opacity-50 mt-5"> 
                <span>53k Views</span>
                <div class="w-1 h-1 rounded-full bg-gray-300"></div>
                <span>2 weeks ago</span>
            </div>
        </div>
    </div>
</template>

<script setup>

    import Avatar from './Avatar.vue'
</script>
