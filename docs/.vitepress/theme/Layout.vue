<!-- .vitepress/theme/Layout.vue -->
<script setup>
import DefaultTheme from 'vitepress/theme'
const { Layout } = DefaultTheme;
const goBack = () =>{
    window.history.go(-1);
}
</script>

<template>
  <Layout>
    <template #sidebar-top>
       <p class="home-link">
           <a href="/">Home</a>
       </p>
    </template>
    <template #page-top>
        <br />
        <a @click="goBack">← Back</a>
    </template>
  </Layout>
</template>

<style>
    .home-link{
        padding:1.6em;
        margin-bottom:.8rem;
        border-bottom:1px dashed #ddd;
    }
</style>