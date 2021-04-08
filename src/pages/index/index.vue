<template>
	<view class="shouye">
		<view class="header">
			<view class="wrap">
					<u-swiper :list="list" indicator-pos="bottomLeft" :effect3d="true" title></u-swiper>
			</view>
		</view>
		<view class="content">
			<view class="content-one">
				
			</view>
			<view class="content-two">
				<view class="top-left"></view>
				<view class="top-right"></view>
				<view class="bottom-left"></view>
				<view class="bottom-right"></view>
			</view>
			
		</view>
		<view class="footer">
			
		</view>
	</view>
</template>

<script>

export default {
	name: '',
	data () {
    	return {
			list: [{
						image: 'https://cdn.uviewui.com/uview/swiper/1.jpg',
						title: '昨夜星辰昨夜风，画楼西畔桂堂东'
					},
					{
						image: 'https://cdn.uviewui.com/uview/swiper/2.jpg',
						title: '身无彩凤双飞翼，心有灵犀一点通'
					},
					{
						image: 'https://cdn.uviewui.com/uview/swiper/3.jpg',
						title: '谁念西风独自凉，萧萧黄叶闭疏窗，沉思往事立残阳'
					}
				],
		}
  	}
}
</script>

<style lang="scss" scoped>
.shouye{
	.header{
		.wrap{
			padding: 40rpx;
		}
	}
	.content{
		display: flex;
		justify-content: space-around;
		.content-one{
			width: 320rpx;
			height: 320rpx;
			background-color: pink;
			border-radius: 40%;
		}
		.content-two{
			width: 320rpx;
			height: 320rpx;
			margin-top: 10rpx;
			//background-color: pink;
			border-radius: 40%;
			display: flex;
			justify-content: space-around;
			flex-flow:row wrap;
			@mixin t1 {
				width:150rpx;
				height:150rpx;
				border-radius: 40%;
				border: 1rpx solid pink;
			}
			.top-left{
				@include t1;
			}
			.top-right{
				@include t1;
			}
			.bottom-left{
				@include t1;
			}
			.bottom-right{
				@include t1;
			}
		}
		
	}
}
</style>
