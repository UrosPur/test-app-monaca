<template>
    <v-ons-page>
        <v-ons-toolbar>
            <div class="center">
                Text input
            </div>
        </v-ons-toolbar>

        <v-ons-list>
            <v-ons-list-item>
                <div class="center">
                    <v-ons-input placeholder="Input your name" float
                                 v-model="name"
                    >
                    </v-ons-input>
                </div>
            </v-ons-list-item>
            <v-ons-list-item>
                <div class="right">
                    Hello {{ name || 'anonymous' }}!
                </div>
            </v-ons-list-item>
        </v-ons-list>
        <div class="left">
            <v-ons-button>button</v-ons-button>
        </div>
    </v-ons-page>
</template>
<script>
    export default {
        created() {

            return {

                name: 'test'
            }
        },
        data() {
            return {
                name: ''
            };
        },
        methods: {
            alert() {
                this.$ons.notification.alert('This is an Onsen UI alert notification test.');
            }
        },

        watch: {}

    };
</script>
