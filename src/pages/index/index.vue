<template>
    <view class="content">
        <wd-select-picker type="radio" label="基本用法" v-model="model.test" :columns="columns"></wd-select-picker>
    </view>
</template>

<script setup>
import { ref } from 'vue'

const model = ref({
    test: '',
})
const columns = ref([
    {
        value: '101',
        label: '男装',
    },
    {
        value: '102',
        label: '奢侈品',
    },
    {
        value: '103',
        label: '女装',
    },
])
</script>

<style>
.content {
    display: flex;
    flex-direction: column;
}
</style>
