<template>
    <b-card>
        <b-card-text>
            {{ user.name }}
        </b-card-text>

        <b-card-text>{{ user.username }}</b-card-text>

        <a href="#" class="card-link">{{ user.email }}</a>
    </b-card>
</template>

<script>
import myApi from "@/api/api.js";
export default {
    name: "Home",
    data() {
        return {
            user: {
                user: "alireza",
            },
        };
    },
    mounted() {
        myApi.get("/users/1").then((response) => (this.user = response.data));
    },
};
</script>

<style></style>
