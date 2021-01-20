<template>
    <div class="k-blocks-field-preview">
        <div v-for="block in value">
            <div class="block-type">{{ block.type }}</div>
            <div class="block-content">
                <component v-if="block.type ==='heading'"
                           v-html="block.content.text"
                           :is="block.content.level"/>
                <div v-else-if="['text', 'list'].indexOf(block.type) !== -1"
                     v-html="block.content.text"/>
                <div v-else-if="block.type === 'video'">{{ block.content.url }}</div>
                <div v-else-if="block.type === 'image'">{{ block.content.src }}</div>
                <pre v-else>{{ block }}</pre>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        value: String,
    },
    computed: {},
    methods: {},
};
</script>
