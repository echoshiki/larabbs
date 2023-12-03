<script setup>
    import { Head } from '@inertiajs/vue3';
    import GuestLayout from '@/Layouts/GuestLayout.vue';
</script>

<template>
    <Head title="Home" />
    <GuestLayout>
    <div class="text-center py-6">
        <h2 class="text-3xl font-bold leading-loose mb-2 after:block after:w-10 after:h-px after:bg-gray-600 after:mx-auto">LaraBBS</h2>
        <div class="text-sm text-light leading-loose text-gray-600">如你所见，这里是用于学习的某个 laravel 系统</div> 
        <div class="flex flex-col gap-2 mt-6">
            <a class="block rounded-md bg-indigo-600 text-white p-4 text-center font-bold hover:opacity-80 duration-500" :href="route('login')">立即登录</a>
            <a class="block rounded-md bg-orange-600 text-white p-4 text-center font-bold hover:opacity-80 duration-500" :href="route('register')">加入我们</a>
        </div>
        <div class="text-sm mt-6">
            <p> Laravel Breeze & Vue</p>
            <p> &copy; 2023 LaraBBS By Shiki All rights reserved </p>
        </div>
    </div>
    </GuestLayout>    
</template>