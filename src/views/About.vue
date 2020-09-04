<template>
    <h1>About</h1>
    <p>{{test}}</p>
</template>

<script lang="ts">
    import { Component, Prop, Vue } from "vue-property-decorator";

    @Component({
        components: {

        }
    })
    export default class About extends Vue {
        @Prop({type: String, required: false})
        test!: string;

        created() {
            console.log("test");
        }
    }
</script>