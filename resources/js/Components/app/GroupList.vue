<script setup >
import { ref } from 'vue';
import TextInput from '../TextInput.vue';
import GroupItem from './GroupItem.vue';

const searchKeyword = ref('');

</script>

<template>
    <div class="px-3">
 <h2 class="text-2xl font-bold mb-4"> My Group</h2>
 <TextInput :model-value="searchKeyword" placeholder="Type to search"/>

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
        </div>
</template>