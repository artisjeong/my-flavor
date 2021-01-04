<template>
    <v-bottom-navigation v-model="index" color="primary" grow>
        <v-btn>
            <v-icon>mdi-home</v-icon>
        </v-btn>

        <v-btn>
            <v-icon>mdi-heart</v-icon>
        </v-btn>

        <v-btn>
            <v-icon>mdi-map-marker</v-icon>
        </v-btn>
        
        <v-btn>
            <v-icon>mdi-account</v-icon>
        </v-btn>
    </v-bottom-navigation>
</template>
<script>
export default {
    name: 'Footer',
    data: () => ({ index: 0 }),
}
</script>