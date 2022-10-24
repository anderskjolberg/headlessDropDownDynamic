<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
import Welcome from '@/Components/Welcome.vue';
import testComponent from '@/Components/TargetComponent.vue';
// import testComponentTwo from '@/Components/TargetComponent2.vue';
</script>

<template>
    <AppLayout title="Input Component">
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Component's
            </h2>
        </template>

        <div class="pt-12 flex h-screen justify-center">
            <!-- <div class="max-w-7xl mx-auto sm:px-6 lg:px-8 h-5/6 flex-grow"> -->
            <div class="max-w-7xl mx-auto lg:px-8 sm:px-6 bg-white shadow-xl sm:rounded-lg mb-24 flex-grow">
                <div class="mt-5">
                </div>
                <div class="grid grid-cols-2">
                    <div>
                        <h1>Drop down liste:</h1>
                        <testComponent />
                    </div>
                </div>
                <!-- <h3>Hello world</h3> -->
            </div>
            <!-- </div> -->
        </div>
    </AppLayout>
</template>
