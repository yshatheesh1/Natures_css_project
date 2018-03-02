Advanced CSS Concepts:

Making an element center relative to parent element
<pre>
<div class="header">
<div class="header-text">hello</div>
</div>


.header{
    position : relative;
    &-text{
        position:absolute;
        top:50%;
        left:50%;
        transform: translateX(-50%)
    }
}

Fill background image in a container
<div class="hello">....something...</div>
.hello{
    background-image : linear-gradient(to right bottom,rgba(red,0.8),rgba(green,0.8)),url('../img.png');
    background-size: cover;
    background-position:top;
}

properties with one value two value and four values

top-50px;right-25px;bottom-50px;left-50px;
padding: 50px 25px 50px 50px;

all four paddings:
padding: 50px; 

top-bottom:50px; left-right:25px;
padding: 50px 25px


Place a section elements on top of image or video
overflow-hidden : makes element fit into section, avoids overflow outside of section


<div class="section">
<div class="bg-video"><video class="bg-video-content" autoplay loop></video></div>
<div class="row">
something
</div>
</div>

.section{
    position:relative;
}

.bg-video{
    position:absolute;
    width:100;
    heigth:100;
    top:0;
    left:0;
    opacity:0.15;
    z-index:-1;
    overflow:hidden;

}


clipping images or div:

clip-path: X Y

 clip-path: polygon(0 0,100% 0,100% 85%,0,100%);
 -webkit-clip-path: polygon(0 0,100% 0,100% 85%,0,100%);

</pre>