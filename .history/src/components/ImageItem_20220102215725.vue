<template>
    <div class="img-item">
        <img src="{{ title }}" alt="{{ title }}" class="img-item__src" />
        <h2 class="img-item__title">{{ titel }}</h2>
    </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
    props: {
        src: String,
        title: String,
    },
})

export default class ImageItem extends Vue {
    src: string;
    title: string;

    set title(str: string) {
        this.title = str;
    }
}

</script>

<style scoped lang="scss">

</style>
