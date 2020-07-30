<template>
    <span>
        <v-navigation-drawer app v-model="drawer" class="white" dark disable-resize-watcher >
            <v-list>
                <template v-for="(item, index) in items">
                    <v-list-tile :key="index">
                        <v-list-tile-content>
                            {{item.title}}
                        </v-list-tile-content>
                    </v-list-tile>
                    <v-divider :key="`divider-${index}`"></v-divider>
                </template>
            </v-list>
        </v-navigation-drawer>
        <v-toolbar app color="white" dark>
            <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-toolbar-side-icon>
                <img alt="Vue logo" width="30px;" src="../assets/logo.png">
                <v-spacer class="hidden-md-and-up"></v-spacer>
                <router-link to="/">
                    <v-toolbar-title style="color: black; margin-left:20px;">Inicio</v-toolbar-title>
                </router-link>
                <v-spacer class="hidden-sm-and-down"></v-spacer>
            <v-btn flat class="hidden-sm-and-down" color="orange">SALIR</v-btn>
        </v-toolbar>
    </span>
</template>

<script>
export default {
    name: 'AppNavigation',
    data() {
        return {
            appTitle: 'Website Horarios',
            drawer: false,
            items: [
                { title: 'Menu' },
                { title: 'Sign In' },
                { title: 'Join' }
            ]
        };
    }
};
</script>

<style scoped>
</style>