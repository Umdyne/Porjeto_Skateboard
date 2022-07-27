<template>
    <div class="flex items-center">
        <div class="bg-orange-500 p-2 rounded-lg">
            <component :is="icon" class="w-4 h-4"/>
        </div>

        <span>
            <slot></slot>
        </span>
    </div>
</template>

<script lang="ts" setup>

    import {defineProps} from "vue";

    defineProps({
        icon: {default: null}
    });
</script>
