<!DOCTYPE html>
<html>
	<head>
	<title> How To Train Your Dragon </title>
	<link rel="stylesheet" href="style.css">
	</head>
	<body>
		<div class="about_dragons">
			<div class="accordion">
				<ul>
					<li>
					<input type="checkbox">
					<span></span>
					<div class="accordion_head">
						<img src="images/Toothless.png">
						<h3>Беззубик</h3>
					</div>
					<div class="accordion_body">
						<img src="images/Toothless_main.jpg">
						<p>Беззубик є одним з найрозумніших з усіх існуючих драконів, а почуттям гумору дуже нагадує Іккінга. Він негативно реагує на будь-які загрози,
						спрямовані на нього і його друзів. Зазвичай цей дракон дуже грайливий і любить побалуватися. Також він дуже цікавий.</p>
					</div>
					</li>
					
					<li>
					<input type="checkbox">
					<span></span>
					<div class="accordion_head">
						<img src="images/Light_Fury.png">
						<h3>Фурія</h3>
					</div>
					<div class="accordion_body">
						<img src="images/Light_Fury_main.jpg">
						<p>Денна Фурія - це маловідомий і вкрай рідкісний вид драконів. Є окремим видом, хоча вони і схожі на Нічну фурію; досить сильний
						і красивий дракон, що належить класу: «Разючі».Денні Фурії, мабуть, один з найпрекрасніших і красивих видів драконів. Особливо виділяється білим мерехтливим
						забарвленням, світло-блакитними очима і абсолютно гладкою лускою, як ніби посипаної маленькими блискітками.</p>
					</div>
					</li>
					
					<li>
					<input type="checkbox">
					<span></span>
					<div class="accordion_head">
						<img src="images/Terrible_Terror.png">
						<h3>Страшний Жах</h3>
					</div>
					<div class="accordion_body">
						<img src="images/Terrible_Terror_main.jpg">
						<p>Страшний Жах - це маленький, стайний, енергійний і товариський дракон, який належить до класу: «Кочегари». Швидше за все, 
						їх прототипом є книжковий Беззубик. Моторошні остраху досить сильно поширені в природі. Їх часто можна зустріти на різних островах архіпелагу.</p>
					</div>
					</li>
					
					<li>
					<input type="checkbox">
					<span></span>
					<div class="accordion_head">
						<img src="images/Stormfly.png">
						<h3>Громгільда</h3>
					</div>
					<div class="accordion_body">
						<img src="images/Stormfly_main.jpg">
						<p>У Громгільди досить доброзичливий характер. Громгільда є вірним і люблячим по відношенню до Астрід драконом. Вона, також, здається, занадто любить Іккінга.
						Хоч вона дуже красива, але не настільки, як небезпечна.Як і всі Злісні Змійовики, Громгільда дуже красивий дракон і, на жаль, вона це знає. Вона має щедру дозу марнославства,
						яке характерно для її виду.</p>
					</div>
					</li>
					
					<li>
					<input type="checkbox">
					<span></span>
					<div class="accordion_head">
						<img src="images/Gronckle.png">
						<h3>Сарделька</h3>
					</div>
					<div class="accordion_body">
						<img src="images/Gronckle_main.jpg">
						<p>Сарделька - мила і добра самка Громмеля. Вона дуже любить Рибьенога. Завдяки їй на йолопи зробили багато зброї з "Заліза Громелля". Зі своїм господарем 
						любить грати в овцебол. А ще любить лизати п'яти Рибьенога перед сном. У неї смішне ім'я через хвоста який товщий ніж у інших Громелей.</p>
					</div>
					</li>
					<li></li>
				</ul>
			</div>
		</div>
	</body>
</html>
@import url('https://fonts.googleapis.com/css2?family=Underdog&display=swap') ;

*{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Underdog', system-ui;
}

.about_dragons {
	min-height: 100vh;
	background-image: url(images/19200626.jpg);
	padding: 30px;
	background-size: cover;
	background-attachment: fixed;
}

.accordion {
	width: 800px;
	margin: 0 auto;
	border: 2px solid #6b537c;
	background-image: linear-gradient(
	to bottom right, 
	#eafc83 0%,
	#9fc6f5 60%, 
	#3366ff 85%, 
	#1f3e9c 100%
	);
}

ul {
	list-style: none;
}

.accordion_head {
	height: 80px;
	padding: 10px 25px;
	cursor: pointer;
	background-color: #6b537c;
	border-top: 1px solid #9775af;
	border-bottom: 1px solid #4f3d5b;
	display: flex;
	align-items: center;
}

.accordion_head h3 {
	color: #f4f4f4;
	font-size: 30px;
	padding-left: 30px;
}

.accordion_head img {
	width: 72px;
}

.accordion_body img {
	float: right;
	padding: 10px;
}

.accordion_body p {
	color: rgba_48, 69, 9, 0.8);
	font-size: 20px;
	padding: 10px 20px;
}

.accordion_body {
	max-height: 0;
	overflow: hidden;
	opacity: 0;
	transition: all .5s ease-in-out;
}

.accordion ul li input:checked ~ .accordion_body {
	max-height: 800px;
	opacity: 1;
}

.accordion ul li input {
	position: absolute;
	height: 80px;
	width: 100%;
	opacity: 0;
	cursor: pointer;
}

.accordion ul li {
	position: relative;
}

.accordion ul li span {
	position: absolute;
	top: 15px;
	right: 30px;
	display: block;
	width: 10px;
	height: 10px;
}


.accordion ul li span::before,
.accordion ul li span::after {
	content: "";position: absolute;
	display: block;
	width: 3px;
	height: 10px;
	background-color: #eee;
	transition: all .5s ease-in-out;
}

.accordion ul li span::before {
	transform: translate(2px, 0) rotate(45deg);
}

.accordion ul li span::after {
	transform: translate(-2px, 0) rotate(-45deg);
}

.accordion ul li input:checked ~ span::before {
	transform: translate(-2px, 0) rotate(45deg);
}

.accordion ul li input:checked ~ span::after {
	transform: translate(2px, 0) rotate(-45deg);
}
