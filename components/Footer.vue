<template>
    <footer class="section">
        <div class="inner clearfix">

            <ul class="site-links float--right">
            <!-- <li><a href="#">Email</a></li>
            <li><a href="#">GitHub</a></li>
            <li><a href="#">Linkedin</a></li>
            <li><a href="#">Twitter</a></li>
            <li><a href="#">Blog</a></li> -->
            <!-- <li><a href="#">About</a></li> -->
            <li>© 2021 Peniel Cho, All Rights Reserved.</li>
            </ul>

            <ul class="site-links float--left">
            <!-- <li>© 2021 Peniel Cho, All Rights Reserved.</li> -->
            <!-- <li><a href="#">Terms</a></li>
            <li><a href="#">Privacy</a></li> -->
            <!-- <li><a href="#">Email</a></li>
            <li><a href="#">Linkedin</a></li>
            <li><a href="#">LINE</a></li> -->
            <li><a href="mailto:mail@penielcho.com">Email</a></li>
            <li><nuxt-link to="/" class="li-alike">Blog</nuxt-link></li>
            <li><a href="https://github.com/thepenielcho" target="blank">GitHub</a></li>
            <li><a href="https://www.linkedin.com/in/peniel-cho/" target="blank">Linkedin</a></li>
            <li><a href="https://twitter.com/ChoPeniel" target="blank">Twitter</a></li>
            <li><a href="https://blog.naver.com/penielcho98" target="blank">Life</a></li>
            </ul>

            <a href="#" class="logo">
            <!-- <svg version="1.0"
                xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                width="24"
                height="24"
                viewBox="0 0 16 16"
                fill="#ccc">
                <path fill-rule="evenodd"
                    d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
            </svg> -->
            <!-- <svg width="100%" height="100%" viewBox="0 0 130 130" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" xmlns:serif="http://www.serif.com/" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">
                <g transform="matrix(4.73424,0,0,4.73424,-145.896,-82.4901)">
                    <text x="31.304px" y="38.437px" style="font-family:'Inter-Regular_Bold', 'Inter', sans-serif;font-size:20.028px;fill:rgb(33,120,255);">P</text>
                    <text x="44.021px" y="38.437px" style="font-family:'Inter-Regular_Bold', 'Inter', sans-serif;font-size:20.028px;">B</text>
                </g>
            </svg> -->
            <svg width="100%" height="100%" viewBox="0 0 130 130" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" xmlns:serif="http://www.serif.com/" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">
                <g transform="matrix(4.73424,0,0,4.73424,-145.896,-82.4901)">
                    <path d="M32.57,38.437L32.57,23.871L38.317,23.871C39.422,23.871 40.363,24.081 41.14,24.501C41.918,24.92 42.512,25.501 42.922,26.243C43.332,26.985 43.537,27.84 43.537,28.807C43.537,29.774 43.329,30.628 42.911,31.367C42.494,32.107 41.891,32.683 41.101,33.095C40.312,33.508 39.358,33.714 38.239,33.714L34.576,33.714L34.576,31.246L37.741,31.246C38.333,31.246 38.823,31.143 39.209,30.937C39.596,30.731 39.885,30.444 40.077,30.076C40.269,29.709 40.365,29.286 40.365,28.807C40.365,28.323 40.269,27.9 40.077,27.537C39.885,27.175 39.595,26.893 39.206,26.691C38.817,26.49 38.324,26.389 37.727,26.389L35.65,26.389L35.65,38.437L32.57,38.437Z" style="fill:rgb(33,120,255);fill-rule:nonzero;"/>
                    <path d="M45.287,38.437L45.287,23.871L51.119,23.871C52.19,23.871 53.084,24.03 53.8,24.348C54.516,24.665 55.054,25.105 55.414,25.667C55.775,26.229 55.955,26.875 55.955,27.605C55.955,28.174 55.841,28.673 55.613,29.102C55.386,29.531 55.074,29.882 54.678,30.155C54.282,30.427 53.831,30.62 53.323,30.734L53.323,30.877C53.878,30.9 54.398,31.057 54.884,31.346C55.37,31.635 55.765,32.039 56.069,32.559C56.372,33.078 56.524,33.695 56.524,34.411C56.524,35.184 56.333,35.873 55.951,36.477C55.57,37.082 55.007,37.559 54.262,37.91C53.518,38.261 52.6,38.437 51.51,38.437L45.287,38.437ZM48.366,35.919L50.877,35.919C51.735,35.919 52.361,35.754 52.754,35.425C53.148,35.095 53.345,34.655 53.345,34.105C53.345,33.702 53.247,33.347 53.053,33.039C52.859,32.73 52.582,32.489 52.225,32.313C51.867,32.138 51.441,32.05 50.948,32.05L48.366,32.05L48.366,35.919ZM48.366,29.966L50.649,29.966C51.071,29.966 51.447,29.892 51.776,29.742C52.106,29.593 52.367,29.381 52.559,29.106C52.751,28.831 52.847,28.501 52.847,28.117C52.847,27.591 52.661,27.166 52.289,26.844C51.916,26.522 51.389,26.36 50.706,26.36L48.366,26.36L48.366,29.966Z" style="fill-rule:nonzero;"/>
                </g>
            </svg>
            </a>

        </div>
    </footer>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
.section {
    position: relative;
    /*absolute가 더 못 올라가게 걸릴 수 있도록!*/
}
.section .inner {
    max-width: 64rem;
    margin: 0 auto;
    box-sizing: border-box;
    position: relative;
    /*포지션이 없는 경우에는 부모요소에 position relative 무조건적으로 추가해주기!*/
}
.clearfix::after{
    content: "";
    clear: both;
    display: block;
}
.float--left {
    float: left;
}
.float--right {
    float: right;
}
footer .inner {
    padding: 50px 0;
    border-top: 1px solid #eee;
}
footer .site-links {
    display: flex;
}
footer .site-links li {
    font-size: 12px;
    margin-right: 10px;
    color: #767676;
    display: inline-block;
}
footer .site-links li a {
    color: #4078c0;
}
footer .site-links li .li-alike{
    color: #4078c0;
}
footer .site-links li a:hover {
    text-decoration: underline;
}
footer .site-links li .li-alike:hover {
    text-decoration: underline;
}
footer .logo {
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    margin: auto;
    width: 24px;
    height: 24px;
    /*완벽히 가운데 배치 not 정렬!*/
}
/* footer .logo:hover svg {
    fill: #4078c0;
} */

</style>