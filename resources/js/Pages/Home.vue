<script setup>
// import GroupList from "../components/app/GroupList.vue";

defineProps({});

</script>

<template>

    <Head title="Social Media App" />

    <div class="grid grid-cols-12 gap-3">
        <div class="col-span-3  py-6 px-3">

            <GroupList />

        </div>


        <div class="col-span-6">
            Posts
        </div>


        <div class="col-span-3">
            Followers
        </div>
    </div>


</template>
