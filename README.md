# jquery.touchSlider
- jQuery 기반의 플리킹 내비게이션 플러그인
- 마크업 요소 선택에 제약이 없으며 초보자도 쉽게 사용하도록 설계
- CSS Selector에 따라 다중 적용 가능
- PC 브라우저에서 드래그로 사용가능 (jquery.event.drag 로드시)
- IE7+ 지원

## Dstyle's Relese
- "jquery 2.1.4" 로 적용.
- autoplay , interval 옵션 추가적용
- autoplay : {boolean} 기본값 false : 자동 플레이 적용
- interval : {millsecend , number} 기본값 3000 : 자동플레이시 간격
- "resize:true" 일 경우, 플리킹 외에 window.resize일 경우에도 height값이 자동적용.
``` js
$("#touchSlider").touchSlider({
	autoplay : true, // 자동 플레이
	interval : 5000 // 5초 단위로 실행
});
```


## 기본구조
``` css
#touchSlider { width:100%; height:150px; background:#ccc; position:relative; overflow:hidden; }
#touchSlider ul { width:99999px; height:150px; position:absolute; top:0; left:0; overflow:hidden; }
#touchSlider ul li { float:left; width:100%; height:150px; font-size:14px; color:#fff; }
```

``` html
<div id="touchSlider">
	<ul>
		<li style="background:#9C9">content 1</li>
		<li style="background:#396">content 2</li>
		<li style="background:#39C">content 3</li>
		<li style="background:#33C">content 4</li>
	</ul>
</div>
```

``` js
$("#touchSlider").touchSlider({
	page : 2
});
```

##Demo
http://dohoons.com/test/flick
