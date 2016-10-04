<template>
	<header class="top-container">
			<div class="topbar-left">
				<ul class="nav-wrap">
					<li v-for="item in leftnavs" class="nav">
					<!-- 这段的意思是如果当面不是魅族商城页面就加上target标签 -->
		            <template v-if="item.name === '魅族商城'">
		              	<a :href="item.sourceUrl" class="nav-name">{{item.name}}</a>
		            </template>
		            <template v-else>
		              <a :href="item.sourceUrl" class="nav-name" target="_blank">{{item.name}}</a>
		            </template>
					</li>
				</ul>
			</div>
			<div class="topbar-right">
				<ul class="nav-info">
					<li v-for="item in rightnavs" class="nav">
					<template v-if="item.name === '我的收藏'">
		              	<a :href="item.sourceUrl" class="nav-name" target="_blank">{{item.name}}
						<div class="topbar-new">new</div>
		              	</a>
		            </template>
		            <template v-else>
		              <a :href="item.sourceUrl" class="nav-name" target="_blank">{{item.name}}</a>
		            </template>
				</ul>
			</div>
  </header>
</template>
<script>
export default {
	data () {
		return {
			leftnavs: [
				{name: '魅族官网', sourceUrl: 'http://www.meizu.com'},
				{name: '魅族商城', sourceUrl: 'http://store.meizu.com/index.html'},
				{name: 'Flyme', sourceUrl: 'http://www.flyme.cn'},
				{name: '专卖店', sourceUrl: 'http://retail.meizu.com/index.html'},
				{name: '服务', sourceUrl: 'http://service.meizu.com/index.html'},
				{name: '社区', sourceUrl: 'http://bbs.meizu.cn'}
			],
			rightnavs: [
				{name:'我的收藏', sourceUrl:"http://me.meizu.com/member/favorite/index"},
				{name:'我的订单', sourceUrl:"http://ordercenter.meizu.com/list/index.html"},
				{name:'登陆', sourceUrl:"https://login.flyme.cn/vCodeLogin?sid=unionlogin&service=store&autodirct=true&useruri=http://store.meizu.com/member/login.htm?useruri=http://store.meizu.com/index.html"},
				{name:'注册', sourceUrl:"https://member.meizu.com/register"},
			]
		}
	}
}
</script>

<style>
.top-container{
	margin:0px;
	padding:0px 80px 0px 40px;
	height:40px;
}
.nav{
	float:left;
}
.nav-wrap{
	float:left;
	display:inline;
	list-style-type: none;
}
.nav-info{
	float: right;
	display:inline;
	list-style-type: none;
}
.nav-name{
    color: #666;
    font-size: 12px;
    margin-right: 40px;
    display: inline-block;
    text-decoration: none;
    transition: color .2s linear;
}
.nav-name:hover{
	color:#00c3f5;
}
.topbar-new {
    position: relative;
    display: inline-block;
    vertical-align: middle;
    color: #fff;
    background-color: #ed4462;
    font-size: 12px;
    margin-left: 5px;
    height: 13px;
    line-height: 10px;
    padding: 0 2px;
    top: -1px;
    border-radius: 2px;
}
.topbar-new:before {
    position: absolute;
    left: -4px;
    top: 2px;
    display: inline-block;
    content: "";
    border-top: 4px solid transparent;
    border-bottom: 4px solid transparent;
    border-right: 6px solid #ed4462;
    width: 0;
    height: 0;
}
</style>
