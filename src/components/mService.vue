<template>
	<div class="site-footer-service">
            <ul class="clearfix">
                <li class="service-item">
                  <span class="service-icon service-icon-seven"></span>
                  <p class="service-desc">
                    <span class="service-desc-bold">7天</span>
                    <span class="service-desc-normal">无理由退货</span>
                  </p>
                </li>
                <li class="service-split-line">
                  <span></span>
                </li>
                <li class="service-item">
                  <span class="service-icon service-icon-fifty"></span>
                  <p class="service-desc">
                    <span class="service-desc-bold">15天</span>
                    <span class="service-desc-normal">换货保障</span>
                  </p>
                </li>
                <li class="service-split-line">
                  <span></span>
                </li>
                <li class="service-item">
                  <span class="service-icon service-icon-one"></span>
                  <p class="service-desc">
                    <span class="service-desc-bold">1年</span>
                    <span class="service-desc-normal">免费保修</span>
                  </p>
                </li>
                <li class="service-split-line">
                  <span></span>
                </li>
                <li class="service-item">
                  <span class="service-icon service-icon-speed"></span>
                  <p class="service-desc">
                    <span class="service-desc-bold">百城</span>
                    <span class="service-desc-normal">速达</span>
                  </p>
                </li>
                <li class="service-split-line">
                  <span></span>
                </li>
                <li class="service-item">
                  <span class="service-icon service-icon-by"></span>
                  <p class="service-desc">
                    <span class="service-desc-bold">全场</span>
                    <span class="service-desc-normal">包邮</span>
                  </p>
                </li>
                <li class="service-split-line">
                  <span></span>
                </li>
                <li class="service-item">
                  <span class="service-icon service-icon-map"></span>
                  <p class="service-desc">
                    <span class="service-desc-bold">2000多家</span>
                    <span class="service-desc-normal">专卖店</span>
                  </p>
                </li>
            </ul>
        </div>
</template>

<script>
	export default {
	data () {
		return {
		}
	}
}
</script>
<style>
.site-footer-service li {
    float: left;
}
/*分割线*/
.service-split-line span {
    display: inline-block;
    height: 44px;
    width: 1px;
    background-color: #e5e5e5;
}
.service-split-line {
    padding-top: 10px;
}
.service-icon {
    display: inline-block;
    height: 36px;
    width: 94px;
    background: no-repeat 50% 50%;
    margin-bottom: 12px;
}
.service-icon-seven {
    background-image: url(http://store.res.meizu.com/resources/php/store/static/common/widgets/site-footer/7.png);
}
.service-icon-fifty {
    background-image: url(http://store.res.meizu.com/resources/php/store/static/common/widgets/site-footer/15.png);
}
.service-icon-one {
    background-image: url(http://store.res.meizu.com/resources/php/store/static/common/widgets/site-footer/1.png);
}
.service-icon-speed {
    background-image: url(http://store.res.meizu.com/resources/php/store/static/common/widgets/site-footer/speed.png);
}
.service-icon-by {
    background-image: url(http://store.res.meizu.com/resources/php/store/static/common/widgets/site-footer/baoyou.png);
}
.service-icon-map {
    background-image: url(http://store.res.meizu.com/resources/php/store/static/common/widgets/site-footer/map.png);
}
.site-footer-service {
    padding: 38px 8px 26px;
    border-bottom: 1px solid #e5e5e5;
}
.service-desc-bold, .service-desc-normal {
    color: #666;
    font-weight: 700;
    font-size: 14px;
}
.service-desc-normal {
    font-weight: 400;
}
.service-item {
    width: 203px;
    text-align: center;
}
</style>