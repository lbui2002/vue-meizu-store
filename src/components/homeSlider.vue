<template>
    <div id="MzHomeSlider" class="home-slider">
        <div class="home-slider-items">
            <div class="bx-wrapper" style="max-width: 100%;">
                <div class="bx-viewport" style="width: 100%; overflow: hidden; position: relative; height: 480px;">
                    <ul class="bxslider" style="width: auto; position: relative;">
                        <li class="home-slider-box" data-bgcolor="#b4d0ea" style="background: rgb(180, 208, 234); float: none; list-style: none; position: absolute; width: 1423px; z-index: 0; display: none;">
                            <a class="home-slider-image" style="width: 1920px; margin-left: -960px;" href="http://hd.meizu.com/sale/nationalday.html?rc=lb1" target="_blank" data-mtype="store_index_ba_1" data-mdesc="第1屏banner">
                                <img src="http://open.file.meizu.com/group1/M00/00/6E/CnQOjVfqFx2AYqroAAcQCeMOVbQ025.png" width="1920" height="480">
                            </a>
                        </li>
                        <li class="home-slider-box" data-bgcolor="#e33e48" style="background: rgb(227, 62, 72); float: none; list-style: none; position: absolute; width: 1423px; z-index: 50; display: list-item;">
                            <a class="home-slider-image" style="width: 1920px; margin-left: -960px;" href="http://detail.meizu.com/item/mx6.html?rc=lb2" target="_blank" data-mtype="store_index_ba_2" data-mdesc="第2屏banner">
                                <img src="http://open.file.meizu.com/group1/M00/00/73/Cix_s1fuEd6AFH-JAA1HC9nUMbw524.png" width="1920" height="480">
                            </a>
                        </li>
                        <li class="home-slider-box" data-bgcolor="#13161f" style="background: rgb(19, 22, 31); float: none; list-style: none; position: absolute; width: 1423px; z-index: 0; display: none;">
                            <a class="home-slider-image" style="width: 1240px; margin-left: -620px;" href="http://detail.meizu.com/item/lexin_mambo.html?rc=lb3" target="_blank" data-mtype="store_index_ba_3" data-mdesc="第3屏banner">
                                <img src="http://open.file.meizu.com/group1/M00/00/68/CnQOjVfiO5uAMYYgAAGhNx9dP1Y307.jpg" width="1240" height="480">
                            </a>
                        </li>
                        <li class="home-slider-box" data-bgcolor="#1b1b1b" style="background: rgb(27, 27, 27); float: none; list-style: none; position: absolute; width: 1423px; z-index: 0; display: none;">
                            <a class="home-slider-image" style="width: 1920px; margin-left: -960px;" href="http://detail.meizu.com/item/meilan_u10.html?rc=lb4" target="_blank" data-mtype="store_index_ba_4" data-mdesc="第4屏banner">
                                <img src="http://open.file.meizu.com/group1/M00/00/6C/CnQOjVfp266AHtXRAATbZQitLA0372.jpg" width="1920" height="480">
                            </a>
                        </li>
                        <li class="home-slider-box" data-bgcolor="#ead68e" style="background: rgb(234, 214, 142); float: none; list-style: none; position: absolute; width: 1423px; z-index: 0; display: none;">
                            <a class="home-slider-image" style="width: 1240px; margin-left: -620px;" href="http://store.meizu.com/item/meizu_ep51.html?rc=lb5" target="_blank" data-mtype="store_index_ba_5" data-mdesc="第5屏banner">
                                <img src="http://storeimg.meizu.com/product/1465731173-65690.jpg" width="1240" height="480">
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="bx-controls bx-has-pager bx-has-controls-direction">
                    <div class="bx-pager bx-default-pager">
                        <div class="bx-pager-item" v-for="n in 5"><a href="" data-slide-index="" class="bx-pager-link">{{n}}</a></div>
                    </div>
                    <div class="bx-controls-direction"><a class="bx-prev" href="">Prev</a><a class="bx-next" href="">Next</a></div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
</script>
<style>
.home-slider {
    height: 480px;
    width: 100%;
    overflow: hidden;
}
</style>
