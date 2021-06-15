<template>
  <div>
    <div class="select_wrap">
      <ul class="default_option">
          <li>
              <div class="option ru">
					  <p>RU</p>
                <div class="icon"></div>
              </div>
          </li>
      </ul>
      <ul class="select_ul">
          <li>
              <div class="option ru">
					 <p>RU</p>
                <div class="icon"></div>
              </div>
          </li>
          <li>
              <div class="option kz">
					  <p>KZ</p>
                <div class="icon"></div>
              </div>
          </li>
          <li>
              <div class="option usa">
					  <p>USA</p>
                <div class="icon"></div>
              </div>
          </li>
          <li>
            <div class="option gb">
					<p>GB</p>
                <div class="icon"></div>
              </div>
          </li>
      </ul>
  </div>
<!-- ====================== -->


  </div>
</template>

<script>
export default {

  head: {
    script: [
      {
        src: "https://code.jquery.com/jquery-3.4.1.min.js",
      },
      {
        type: 'text/javascript',
        src: '/js/my.js',
        body: true
      }
    ]
  }
}
</script>

<style>
.select_wrap{
 width: 130px;
  margin: auto;
  position: relative;
  user-select: none;
  margin-left: 20px;
}

.select_wrap .default_option{
  background: #F8F8F8;
  border-radius: 5px;
  border: 1px solid #E4E4E4;
  position: relative;
  cursor: pointer;
}

.select_wrap .default_option li{
    padding: 16px 20px;
}

.select_wrap .default_option:before{
    content: "";
    position: absolute;
    top: 18px;
    right: 18px;
    width: 6px;
    height: 6px;
    border: 2px solid;
    border-color: transparent transparent #555555 #555555;
    transform: rotate(-45deg);
}

.select_wrap .select_ul{
  position: absolute;
  top: 55px;
  left: 0;
  width: 100%;
  background: #fff;
  border-radius: 5px;
  display: none;
}

.select_wrap .select_ul li{
  padding: 10px 20px;
  cursor: pointer;
}

.select_wrap .select_ul li:first-child:hover{
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}

.select_wrap .select_ul li:last-child:hover{
  border-bottom-left-radius: 5px;
  border-bottom-right-radius: 5px;
}

.select_wrap .select_ul li:hover{
  background: #fff4dd;
}

.select_wrap .option{
  display: flex;
  align-items: center;
}

.select_wrap .option p {
font-style: normal;
font-weight: 600;
font-size: 14px;
line-height: 20px;
text-align: center;
/* black */
color: #212121;
}

.select_wrap .option .icon{
  background: url('https://res.cloudinary.com/poliweb/image/upload/v1623399248/new_projelt/flags_d0dtdt.png') no-repeat 0 0;
	background-size: 400px 375px;
	width: 24px;
	height: 16px;
  margin-right: 15px;
	margin-left: 15px;
}

.select_wrap .option.ru .icon{
  background-position: -175px -279px;
	box-shadow: 0px 0px 10px 1px rgba(0,0,0,0.35);
}

.select_wrap .option.kz .icon{
  background-position:  -175px -179px;
}

.select_wrap .option.usa .icon{
  background-position: -350px -329px;
}

.select_wrap .option.gb .icon{
 background-position: -250px -104px;
}

.select_wrap.active .select_ul{
  display: block;
}

.select_wrap.active .default_option:before{
  top: 25px;
  transform: rotate(-225deg);
}

/* ================================= */
.select {
	margin: 0 auto;
	width: 250px;
	position: relative;
}

.select.is-active .select__body {
	display: block;
}

.select__header {
	border: 1px solid #ccc;
	display: flex;
	cursor: pointer;
}

.select__body {
	display: none;
	position: absolute;
	left: 0;
	right: 0;
	top: 100%;
	border: 1px solid #ccc;
	border-top: 0;
}

.select__icon {
	display: flex;
	flex-shrink: 0;
	align-items: center;
	justify-content: center;
	text-align: center;
	margin-left: auto;
	width: 40px;
	height: 40px;
}

.select__current {
	font-size: 18px;
	line-height: 24px;
	padding: 8px;
}

.select__item {
	cursor: pointer;
	font-size: 16px;
	line-height: 24px;
	padding: 8px;
}

.select__item:hover {
	background: #ccc;
}
</style>
