<script setup >
import GroupItem from '../Components/app/GroupItem.vue';
import TextInput from '../Components/TextInput.vue';

const searchKeyword = ref('');

</script>

<template>
 <h2 class="text-2xl font-bold px-3"> My Group</h2>
 <TextInput :model-value="searchKeyword" />

            <div class="py-8">
                <div v-if="false" class="text-gray-400 flex text-center">
                    You are not joined to any groups
                </div>
                <div v-else>
                    
                    <GroupItem  
                    image="https://picsum.photos/100" 
                    title="Laravel Developer"
                    description="Lorem ipsum dolor sit amet, consectetur."
                    />
                    <GroupItem  
                    image="https://picsum.photos/100" 
                    title="Vue js Developer"
                    description="Lorem ipsum dolor sit amet, consectetur."
                    />

                </div>
            </div>
</template>