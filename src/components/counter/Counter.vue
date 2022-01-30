<template>
    <div>It's Counter component</div>
    <div>{{ count }}</div>
    <button @click="increment">+1</button>
</template>

<script lang="ts">
import { Vue, Options } from "vue-class-component";

@Options({})
export default class Counter extends Vue {
    count = 0;

    increment() {
        this.count++;
    }
}
</script>
