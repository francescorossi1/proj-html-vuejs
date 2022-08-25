<template>
    <div class="text-center m-auto container-fluid">
        <div>
            <h2 class="display-1"><strong>Latest News & Our <span class="tc-lime">Blog</span></strong></h2>
        </div>
        <LimeBreak class="justify-content-center" />
        <div class="row">
            <div class="col-4" v-for="post in posts" :key="post.id">
                <BlogPost :post="post" />
            </div>
        </div>
        <BaseButton text='VIEW ALL POSTS' class="lime-button mb-5" />
        <div class="d-flex row">

        </div>
    </div>
</template>

<script>
import LimeBreak from './LimeBreak.vue';
import BaseButton from './BaseButton.vue';
import BlogPost from './BlogPost.vue';
export default {
    name: 'BlogSection',
    components: { LimeBreak, BaseButton, BlogPost },
    data() {
        return {
            posts: [
                { id: 1, src: 'blog-1.jpg', date: 'May 24, 2018', author: 'Alex', title: 'Marketing Ideas' },
                { id: 2, src: 'blog-2.jpg', date: 'May 24, 2018', author: 'Alex', title: 'Rest During Working Hours' },
                { id: 3, src: 'blog-3.jpg', date: 'May 24, 2018', author: 'Alex', title: 'Develop Your Startup Idea' }
            ]
        }
    }
}
</script>

<style>
</style>