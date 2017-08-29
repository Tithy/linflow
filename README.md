移动横向瀑布流--

8.29更新
-重新定义入口文件
-重新计算排列入口
需要定义：隐藏图片容器/显示图片容器/设备宽度/随机高度

在使用中可将高度设定为固定值

var $linnflow = $(".m-content-list").iFlow({

    FloWidth:document.documentElement.clientWidth,//设备宽度
    
    FloNum:100,//固定高度
    
    /*randomNum:Math.random() * (boxW*0.625-50+1)+50;,随机高度*/
    
    FloImg:$(".s-imglist-none"),//隐藏图片容器
    
    FLOTime:50,
    
    success:function (Lin) {
    
        beginSwiper(Lin);//引用第三方swiper进入大图浏览模式
        
  }
  
});

linflow.js


    var FloP = LinNode.parents(".m-content-item");//显示图片容器
    
//烦请大佬们指正
