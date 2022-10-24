<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
import Welcome from '@/Components/Welcome.vue';
import testComponent from '@/Components/TargetComponent.vue';
</script>

<template>
    <AppLayout title="Input Component">
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Input Component
            </h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                <div class="bg-white overflow-hidden shadow-xl sm:rounded-lg">
                    <testComponent class="z-50" />
                    <h3>Hello world</h3>
                </div>
            </div>
        </div>
    </AppLayout>
</template>
