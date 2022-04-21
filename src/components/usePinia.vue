<template>
    <div>{{ userStore.name }}</div>
    <div @click="update">修改名称</div>
</template>

<script lang="ts" setup>
import { useUserStore } from '@/store/user'

const userStore = useUserStore()

const update = () => {
    userStore.updateName('飞天老李')
}
</script>

