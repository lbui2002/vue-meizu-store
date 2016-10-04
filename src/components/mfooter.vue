<template>
<div class="mzcontainer">
	<m-service></m-service>
	<div class="site-footer-navs clearfix">
		<div v-for="item in cols" class="footer-nav-item">
			<h4 class="footer-nav-title">{{item.lists.name}}</h4>
			<ul>
				<li v-for="sub in item.lists.subs">
					<!--嵌套的循环不用在额外加上父类循环的属性名，直接child.key就可以了 -->
	          		<template v-if="sub.name === '官方微信'">
		              	<a class="meizu-footer-wechat">{{sub.name}}
						<img src="http://www2.res.meizu.com/zh_cn/images/common/weixin.png?v=2015" alt="微信二维码">
		              	</a>
		            </template>
		            <template v-else>
		            	<a target="_bank" :href="sub.url" >{{sub.name}}</a>
		            </template>
	          	</li>
          	</ul>
		</div>
		<div class="footer-nav-custom">
                <h4 class="nav-custom-title">24小时全国服务热线</h4>
                <a href="tel:400-788-3333"><h3 class="nav-custom-number">400-788-3333</h3></a>
                <a class="nav-custom-btn" href="javascript:void(0);" onclick="window.open('http://live-i.meizu.com/live800/chatClient/chatbox.jsp?companyID=8957&amp;configID=4&amp;enterurl='+ encodeURIComponent(document.URL) + '&amp;pagereferrer=' + encodeURIComponent(document.referrer) + '&amp;info=&amp;k=1', '_blank','height=775,width=1200,fullscreen=3,top=100,left=100,status=yes,toolbar=no,menubar=no,resizable=no,scrollbars=no,location=no,titlebar=no,fullscreen=no');">
                    <img src="http://store.res.meizu.com/resources/php/store/static/common/widgets/site-footer/20x21xiaoshi.png" width="20" height="21">
                    24小时在线客服
                </a>
            </div>
	</div>
	<bottom-bar></bottom-bar>
	</div>
</template>
<script>
import bottomBar from './bottomBar'
import mService from './mService'
export default {
	data () {
		return {
			cols:[
				    {
				        "lists": {
				            "name": "帮助说明",
				            "subs": [
				                {
				                    "name": "支付方式",
				                    "url": "http://store.meizu.com/explain/payment_help.html"
				                },
				                {
				                    "name": "配送说明",
				                    "url": "http://store.meizu.com/explain/deliverynote.html"
				                },
				                {
				                    "name": "售后服务",
				                    "url": "http://store.meizu.com/explain/warranty_services.html"
				                },
				                {
				                    "name": "付款帮助",
				                    "url": "http://store.meizu.com/explain/payment_helps.html"
				                }
				            ]
				        }
				    },
				    {
				        "lists": {
				            "name": "Flyme",
				            "subs": [
				                {
				                    "name": "开放平台",
				                    "url": "https://open.flyme.cn/"
				                },
				                {
				                    "name": "固件下载",
				                    "url": "http://www.flyme.cn/firmware.jsp"
				                },
				                {
				                    "name": "软件商店",
				                    "url": "http://app.flyme.cn/"
				                },
				                {
				                    "name": "查找手机",
				                    "url": "http://finder.flyme.cn/"
				                }
				            ]
				        }
				    },
				    {
				        "lists": {
				            "name": "关于我们",
				            "subs": [
				                {
				                    "name": "关于魅族",
				                    "url": "http://www.meizu.com/about.html"
				                },
				                {
				                    "name": "加入我们",
				                    "url": "http://hr.meizu.com/"
				                },
				                {
				                    "name": "联系我们",
				                    "url": "http://www.meizu.com/contact.html"
				                },
				                {
				                    "name": "法律声明",
				                    "url": "http://www.meizu.com/legalStatement.html"
				                }
				            ]
				        }
				    },
				    {
				        "lists": {
				            "name": "关注我们",
				            "subs": [
				                {
				                    "name": "新浪微博",
				                    "url": "http://weibo.com/meizumobile"
				                },
				                {
				                    "name": "腾讯微博",
				                    "url": "http://t.qq.com/meizu_tech"
				                },
				                {
				                    "name": "QQ空间",
				                    "url": "http://user.qzone.qq.com/2762957059"
				                },
				                {
				                    "name": "官方微信",
				                    "url": "#"
				                }
				            ]
				        }
				    } 
				]
		}
	},
	components: {
		bottomBar,
		mService
	}
}
</script>

<style>
.mzcontainer {
    width: 1240px;
    margin: 0 auto;
}
.mzcontainer::before, .mzcontainer::after,.clearfix:before, .clearfix:after {
    content: " ";
    display: table;
}
.clearfix:after {
    content: " ";
    clear: both;
    height: 0;
    visibility: hidden;
    display: block;
}
.clearfix {
     zoom: 1; 
}
h1, h2, h3, h4, h5, h6, ul, ol, dl, dt, dd, p{
	margin: 0;
    padding: 0;
    list-style: none;
    font-weight: 400;
}
h4,{
	display: block;
	-webkit-margin-before: 1.33em;
    -webkit-margin-after: 1.33em;
    -webkit-margin-start: 0px;
    -webkit-margin-end: 0px;
}
.site-footer-navs {
    padding: 30px 0;
    margin-right: -10px;
}
.footer-nav-custom,.footer-nav-item {
    float: left;
    width: 244px;
    text-align: center;
    margin-right: 5px;
}
.nav-custom-title,.footer-nav-title {
	font-size: 14px;
	color: #333;
	margin-bottom: 10px;
}
.footer-nav-item li {
    line-height: 22px;
}
.footer-nav-item li a {
    font-size: 12px;
    color: #666;
    transition: color .2s linear;
}
.footer-nav-item li a:hover {
    color: #00c3f5;
}
a {
    text-decoration: none;
    outline: 0;
    background: transparent;
}
li{
	display: list-item;
	text-align: -webkit-match-parent;
}
.nav-custom-number {
    color: #1fa7ea;
    font-size: 24px;
    margin: 20px 0 14px;
}
h3 {
    display: block;
    -webkit-margin-before: 1em;
    -webkit-margin-after: 1em;
    -webkit-margin-start: 0px;
    -webkit-margin-end: 0px;
}
.nav-custom-btn {
    display: inline-block;
    width: 160px;
    height: 34px;
    line-height: 34px;
    text-align: center;
    text-decoration: none;
    color: #fff;
    background-color: #1fa7ea;
    border-radius: 2px;
    font-size: 12px;
    transition: all .2s linear;
}
.nav-custom-btn:hover {
    background-color: #4dcff6;
}
.nav-custom-btn img {
    vertical-align: middle;
}
img[Attributes Style] {
    width: 20px;
    height: 21px;
}
a:active, a:hover {
    outline: 0;
}

/*鼠标指向，弹出*/
.meizu-footer-wechat {
    position: relative;
}
.meizu-footer-wechat:hover img {
    display: block;
}
.meizu-footer-wechat img {
    position: absolute;
    z-index: 999;
    width: 249px;
    top: -190px;
    left: 32px;
    display: none;
}
img {
    vertical-align: top;
}
</style>