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

    protected src: string;

    protected title: string;

    constructor(src: string, title: string) {
        super();
        this.src = src;
        this.title = title;
    }
}

</script>

<style scoped lang="scss">

</style>
