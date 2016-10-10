# Simple-Easy-Slider
A simple jquery based slider for your web page. With a very light code, and easy instalation, it can be set up to fit any size easily.

Intructions

1. Insert jquery library and plugin
Just insert the plugin .js file after jquery.

<script  src="./js/jquery-1.10.2.min.js"></script>
<script  src="./js/SimpleEasySlider1.1.js"></script>
			
2. Slider HTML
Insert this HTML in your page, put the pictures inside "slides" div, you can load as many pictures as wanted. you can also have a title and a subtitle for each slide


<div class="slider">
<div class="sliderControll"><div class="SlNextBT"></div><div class="SlPreviousBT"></div></div>
		
	<div class="slides">

        <!--Insert your images here -->

		<div><img src="img/img0.jpg" ><p class="sliderTitle">A Simple Title</p><p class="sliderSubTitle">An Easy Subtitle</p><span class="sliderOverlay"></span></div>
		<div><img src="img/img1.jpg"><p class="sliderTitle">A Simple Title</p><p class="sliderSubTitle">An Easy Subtitle</p><span class="sliderOverlay"></span></div>
		<div><img src="img/img2.jpg" ><p class="sliderTitle">A Simple Title</p><p class="sliderSubTitle">An Easy Subtitle</p><span class="sliderOverlay"></span></div>
		<div><img src="img/img3.jpg" ><p class="sliderTitle">A Simple Title</p><p class="sliderSubTitle">An Easy Subtitle</p><span class="sliderOverlay"></span></div>
		<div><img src="img/img4.jpg" ><p class="sliderTitle">A Simple Title</p><p class="sliderSubTitle">An Easy Subtitle</p><span class="sliderOverlay"></span></div>   
		<div><img src="img/img5.jpg" ><p class="sliderTitle">A Simple Title</p><p class="sliderSubTitle">An Easy Subtitle</p><span class="sliderOverlay"></span></div> 
	</div>
	
</div>

3. Slider CSS
Insert the link of the css file in your page. You can change the slider class to fit the height and width wanted.

.slider {
    width:100%;
    height:500px;
    margin:0 auto;
    background-color:white;
    overflow: hidden;
}
			
4. Options
You are done with the basic setup, Title, subtitle, color overlay efect and navigation can be easily turned off by easyOptions() function. Just write it on your page after the plugin .js file.

<script>
  easyOptions(true, false, false, false);
</script>
			
Here is how it works:

function sliderOptions(title, subTitle, overlay, control) {
    if ( ! title && ! subTitle && ! overlay && ! control) {
        $(".sliderTitle, .sliderSubTitle, .sliderOverlay, .sliderControll").css("display","none");
            return;
    }

        $(".sliderTitle, .sliderSubTitle, .sliderOverlay, .sliderControll").css("display","block");
    }

easyOptions(true, false, false, false);
