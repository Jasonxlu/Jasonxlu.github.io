---
layout: nofooterpage
title: Mother's Day 
image: 
description: To Mom
nav-menu: False
---

<img class="center" src="assets/images/hmd2.png" style="width:50%; height:50%;">
<p class= "center2" id ="para">
<strong>Dear Mom, <br/><br/>

&emsp;&emsp;I'm sorry I can't spend mother's day with you at home this year and I rarely call due to how busy I am. 
Thank you so much for being such a great mother. I know you are also super busy, but be sure to take care of yourself
and get some good rest. I hope you have a wonderful day. I miss you and I love you. <br/><br/>

Happy Mother's Day! 

<br/><br/>
Your son, </strong>

</p>

<img class="offset" src="assets/images/sig.png" style="width:25%; height:25%;">

<div class="content">
			<div class="inner">
					<a onclick="change()" class="button special icon fa-language" id="lang">中文</a>
			</div>
        </div>

<style>
    .center {
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 50%;
        margin-top: 50px;
        margin-bottom: 25px;
        padding-right: 50px;
        padding-left: 50px;
    }
    .center2 {
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 50%;
        margin-top: 50px;
        margin-bottom: 25px;
        padding-right: 50px;
        padding-left: 50px;
        line-height: 2;
    }
    
    .offset {
        display: block;
        margin-left: auto;
        margin-right: 50%;
        width: 50%;
        margin-top: 0px;
        margin-bottom: 25px;
        padding-right: 50px;
        padding-left: 50px;
    }

</style>

<script>
function change() {
    var btn = document.getElementById("lang");
    
    if(btn.innerHTML == "中文") {
        btn.innerHTML = 'English';
        para.innerHTML = "亲爱的妈妈, <br/><br/>&emsp;&emsp;很抱歉今年不能在家陪你过母亲节，也因为忙所以很少打电话。非常感谢您成为如此伟大的母亲。我知道你也很忙，但一定要照顾好自己，好好休息。我希望你有一个美好的一天。我想你，我爱你。<br/><br/>母亲节快乐！ <br/><br/>你的儿子, ";
    }
    else {
        btn.innerHTML = "中文"
        para.innerHTML = "<strong>Dear Mom, <br/><br/>&emsp;&emsp;I'm sorry I can't spend mother's day with you at home this year and I rarely call  due to how busy I am. Thank you so much for being such a great mother. I know you are also super busy, but be sure to take care of yourself and get some good rest. I hope you have a wonderful day. I miss you and I love you. <br/><br/>Happy Mother's Day! <br/><br/>Your son, </strong>"
    }
}
</script>
