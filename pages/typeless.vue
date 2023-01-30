<template>
    <div>noop</div>
</template>

<script>
export default {
    props: {
        tracks: {
            /** @type {import('vue').PropType<MyNamespace.Track[]>} */
            type: Array,
            required: true,
        },
    },
    data() {
        return {
            inputs: this.tracks.map(track => track),
        };
    },
};
</script>
