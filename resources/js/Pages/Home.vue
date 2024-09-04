<script setup>
import { Head, Link } from '@inertiajs/vue3';

defineProps({
    canLogin: {
        type: Boolean,
    },
    canRegister: {
        type: Boolean,
    },
    laravelVersion: {
        type: String,
        required: true,
    },
    phpVersion: {
        type: String,
        required: true,
    },
});

function handleImageError() {
    document.getElementById('screenshot-container')?.classList.add('!hidden');
    document.getElementById('docs-card')?.classList.add('!row-span-1');
    document.getElementById('docs-card-content')?.classList.add('!flex-row');
    document.getElementById('background')?.classList.add('!hidden');
}
</script>

<template>
    <Head title="Social Media App" />
   
    <div class="grid grid-cols-12 gap-3">
    <div class="col-span-3">
        <h2> My Group</h2>
        <div>
            You are not joined to any groups
        </div>
        <div>
            <div class="flex">
                <img src="https://picsum.photos/100" alt="">
                <div>
                    <h3>Laravel Developer</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur.</p>
                </div>
            </div>
        </div>
    </div>
    <div class="col-span-6">
        Posts
    </div>
    <div class="col-span-3">
        Followers
    </div>
</div>


</template>
