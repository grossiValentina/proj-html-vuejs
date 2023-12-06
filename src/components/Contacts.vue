<script>

export default {
    props: {
        contact: {
            type: String,

        }
    },
}
</script>


<template>
    <div>
        <p><i class="icon fa-solid fa-phone mb-0 px-1"></i>+1(305)1234-5678</p>
        <p><i class="icon fa-solid fa-envelope px-1"></i>hello@example.com</p>
    </div>
</template>


<style scoped lang="scss">
@use "./style/partials/variables" as *;

.icon {
    color: $White;
}

p {
    color: $White;
}
</style> 