<template>
    <panel-outer-container containerClass="w-1/2 mr-12">
        <panel componentClass="h-40">
            <template v-slot:header>
                <h1 class="text-white text-xl">{{ title }}</h1>
            </template>

            <template v-slot:body>
                <p>{{ description }}</p>
            </template>
        </panel>
    </panel-outer-container>
</template>

<script>
export default {
    data() {
        return {
            title: 'Hot Tips',
            description: "Don't burn the onions",
            componentClass: 'h-60'
        }
    },
    props: {
        recipe: {},
    }
}
</script>
