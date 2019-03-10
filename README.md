# 移动端项目豆瓣电影

效果预览：[点击查看](https://x1059455449.github.io/doubanmovie/index.html)

## API

> 获取 Top250的电影

支持 JSONP

[http://api.douban.com/v2/movie/top250?start=0&count=10&callback=fn](http://api.douban.com/v2/movie/top250?start=0&count=10&callback=fn)

范例：

	$.ajax({
	          url: '//api.douban.com/v2/movie/top250',
	          data: {
	            start: 0,
	            count: 10
	          },
	          dataType: 'jsonp'
	        }).done(function(ret){
	
	        })

>获取榜单

支持 JSONP

[http://api.douban.com/v2/movie/us_box?start=0&count=10&callback=fn](http://api.douban.com/v2/movie/us_box?start=0&count=10&callback=fn)

范例

	$.ajax({
	          url: '//api.douban.com/v2/movie/us_box',
	          data: {
	            start: 0,
	            count: 10
	          },
	          dataType: 'jsonp'
	        }).done(function(ret){
	
	        })

>搜索

支持 jsonp

[http://api.douban.com/v2/movie/search?q=冬天](http://api.douban.com/v2/movie/search?q=冬天)

        $.ajax({
          url: 'http://api.douban.com/v2/movie/search',
          data: {
            q: '冬天'
          },
          dataType: 'jsonp'
        }).done(function(ret){

        })


## 提示

如果效果中图片展示不出来，可在 html 添加 meta

	<meta name="referrer" content="never">