<template>
    <div class="prevnext-container">
        <NuxtLink class="prev-container" v-if="prev" :to="{ name: 'slug', params: { slug: prev.slug } }">
            <div class="prev-nav">Previous Post</div>
            <div class="prev-link">{{ prev.title }}</div>
        </NuxtLink>
        <nuxt-link v-else to='/' class="prev-container">
                    <div class="prev-nav">No Previous Post</div>
                    <div class="prev-link">
                        <span>홈으로 돌아가기</span>
                    </div>
        </nuxt-link>
        <NuxtLink class="next-container" v-if="next" :to="{ name: 'slug', params: { slug: next.slug } }">
            <div class="next-nav">Next Post</div>
            <div class="next-link">{{ next.title }}</div>
        </NuxtLink>
        <nuxt-link v-else to='/' class="next-container">
            <div class="next-nav">No Next Post</div>
            <div class="next-link">
                <span>홈으로 돌아가기</span>
            </div>
        </nuxt-link>
    </div>
</template>

<script>
    export default {
        props: {
        prev: {
            type: Object,
            default: () => null
        },
        next: {
            type: Object,
            default: () => null
        }
        }
    }
</script>

<style scoped>
.clearfix::after{
    content: "";
    clear: both;
    display: block;
}
.prevnext-container{
    display: flex;
    justify-content: space-between;
    margin: 4rem auto;
    /* background-color: lightsteelblue; */
    max-width: 800px;
}
.prev-container{
    padding: 2.3rem 3rem;
    width: 45%;
    background-color: #F2F4F6;
    
    border-radius: 1rem;
}
.prev-container:hover{
    background-color: #E7F3FF;
    transition: 0.3s;
}
.prev-container:hover > .prev-nav{
    color: #3182F6;
    transition: 0.3s;
}
.prev-container:hover > .prev-link{
    color: #3182F6;
    transition: 0.3s;
}
.prev-container .prev-nav{
    color: #444F61;
    font-weight: 600;
    font-size: 1.35rem;
    margin: 0 0 1rem;
}
.prev-container .prev-link{
    color: #333D4B;
    font-weight: 400;
    font-size: 1.1rem;
    word-break: keep-all;
    line-height: 1.3;
    display: block;
}
.next-container{
    padding: 2rem 4rem;
    width: 45%;
    background-color: #F2F4F6;
    border-radius: 1rem;
}
.next-container:hover{
    background-color: #E7F3FF;
    transition: 0.3s;
}
.next-container:hover > .next-nav{
    color: #3182F6;
    transition: 0.3s;
}
.next-container:hover > .next-link{
    color: #3182F6;
    transition: 0.3s;
}
.next-container .next-nav{
    color: #444F61;
    font-weight: 600;
    font-size: 1.35rem;
    margin: 0 0 1rem;
    float: right;
    text-align: right;
    width: 100%;
}
.next-container .next-link{
    color: #333D4B;
    float: right;
    font-weight: 400;
    font-size: 1.1rem;
    text-align: right;
    word-break: keep-all;
    line-height: 1.3;
}
.next-container span{
    float: right;
    text-align: right;
}
</style>