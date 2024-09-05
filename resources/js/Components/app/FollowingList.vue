<script setup >
import { ref } from 'vue';
import TextInput from '../TextInput.vue';
import FollowingItem from './FollowingItem.vue';

const searchKeyword = ref('');

</script>

<template>
    <div class="px-3">
 <h2 class="text-2xl font-bold mb-4"> My Friend</h2>
 <TextInput :model-value="searchKeyword" placeholder="Type to search"/>

            <div class="py-8">
                <div v-if="false" class="text-gray-400 flex text-center">
                    You don't have friends yet.
                </div>
                <div v-else>
                    
                    <FollowingItem  
                    image="https://picsum.photos/100" 
                    title="Jon Doe"
                    />
                    <FollowingItem  
                    image="https://picsum.photos/100" 
                    title="Elon Musk"
                    />

                </div>
            </div>
        </div>
</template>