<template>
    <el-button href="/login/google"
            @click="openGoogle"
            plain
            :size="size">
        <i class="v-icon v-google"></i>
        Connect with your
        <span class="go-primary">G</span><span class="go-red">o</span><span class="go-yellow">o</span><span class="go-primary">g</span><span class="go-green">l</span><span class="go-red">e</span>
        account
    </el-button>
</template>

<script>
    export default {
        props: {
            size: {
                type: String,
                default: 'medium',
            },
        }, 

        methods: {
            openGoogle() {
                window.location = '/login/google'; 
            }
        }
    };
</script>
