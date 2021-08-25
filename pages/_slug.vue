<template>
    <article>
        <!-- <img :src="require(`~/assets/resources/${article.img}`)" alt="" class="main-article-image" /> -->
        <h1 class="article-title">{{article.title}}</h1>
        <p class="dateby">{{article.datetime}} · by {{article.author}}</p>
        <img :src="require(`~/assets/resources/${article.img}`)" alt="" class="main-article-image" />
        <nuxt-content :document="article" />
        <!-- <Prevnext /> -->

        <Prevnext :prev="prev" :next="next" />
    </article>
</template>

<script>
// import Prevnext from '~/components/Prevnext.vue';
export default {
    // components: { Prevnext },
    async asyncData({ $content, params }) {
        const article = await $content('blog', params.slug)
        .fetch();

        const [prev, next] = await $content('blog')
        .only(['title', 'slug'])
        .sortBy('datetime', 'desc')
        .surround(params.slug)
        .fetch()

        return { article, prev, next }
    }
}
</script>

<style scpoed>
    article {
        display: block;
        margin: 0 auto;
        padding: 50px 30px;
        max-width: 800px;
    }
    article h1 {
        font-size: 2.5rem;
        font-weight: 600;
        margin: 2.3rem auto 0;
        color: #333D4B;
        text-align: center;
    }
    article .dateby{
        font-weight: 500;
        text-align: center;
        margin: 1.4rem 0 2.5rem;
    }
    article .main-article-image{
        margin: 2rem 0 5rem;
    }
    article h2{
        font-size: 1.55rem;
        margin: 1.5rem 0;
        color: #333D4B;
        font-weight: 500;
    }
    article h3 {
        font-size: 1.3rem;
        margin: 1.3rem 0 1.3rem;
        color: #333D4B;
        font-weight: 500;
    }
    article p {
        font-weight: 300;
        font-size: 1.15rem;
        text-decoration: none;
        color: #6B7684;
        line-height: 1.8;
        word-break: keep-all;
    }
    article img {
        display: block;
        max-width: 740px;
        margin: 2rem auto;
        box-sizing: border-box;
        border-radius: 1rem;
    }
    article a {
        text-decoration: none;
    }
</style>