<template>
    <div class="d-flex justify-content-between align-items-center">
        <b-nav small>
            <b-nav-item active>Active</b-nav-item>
            <b-nav-item>Link</b-nav-item>
            <b-nav-item>Another Link</b-nav-item>
            <b-nav-item disabled>Disabled</b-nav-item>
        </b-nav>
        <img src="@/assets/logo.png" width="50px" alt="" />
    </div>
</template>

<script>
export default {
    name: "Header",
};
</script>

<style></style>
