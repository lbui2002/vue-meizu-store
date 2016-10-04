<template>
    <div class="site-gotop" style="display: block;">
        <a class="gotop-suggest" title="建议反馈" href="http://me.meizu.com/member/advice/index" target="_blank"></a>
        <div class="gotop-arrow" title="回到顶部"></div>
    </div>
</template>
<script>
	
</script>
<style>
.site-gotop {
    position: fixed;
    width: 44px;
    bottom: 50px;
    left: 50%;
    margin-left: 640px;
    display: none;
}
.gotop-suggest, .gotop-arrow {
    display: inline-block;
    width: 44px;
    height: 44px;
    background: #b4b4b4 no-repeat 50% 50%;
    cursor: pointer;
}
.gotop-suggest {
    background-image: url(http://store.res.meizu.com/resources/php/store/j/home/widgets/home-gotop/suggest.png);
}
.gotop-arrow {
    background-image: url(http://store.res.meizu.com/resources/php/store/j/home/widgets/home-gotop/gotop-arrow.png);
    margin-top: 5px;
}
</style>