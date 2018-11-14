页面meta设置 
 
HTML使用方法: 
是否启用Ie6提示：<meta name="ie6Prompts" content="true" /> 
是否禁用鼠标右键：<meta name="rightMouseButton" content="true" /> 
是否启用返回顶部按钮：<meta name="toTop" content="true" /> 
是否启用版权信息：<meta name="Copyright" content="true" /> 
是否启用双击滚屏：<meta name="DClickScrolling" content="true" /> 
是否启用网站变灰：<meta name="GrayPage" content="true" /> 
是否开启网站维护中提示灰：<meta name="Egis" content="true" />

==========================================================

截取字符串 
 
HTML使用方法: 
<img dsh="limit" num="10" ></li> 
 
JS使用方法 
$('div,p,li,span...').limit('8');

==========================================================

等比例缩放图片 
 
HTML使用方法:
<p dsh="imgAuto" width="80" height="100" > <img src="..."><;/li> </p> 
  
JS使用方法 
$('img,div img,p img,li img,span img...').imgAuto(80,100);

==========================================================

获取系统时间 
 
HTML使用方法: 
<div dsh="time" wel="欢迎光临，今天是：">正在加载...</div>  
<input type="text" dsh="time" value="正在加载..."> 
  
JS使用方法
div等元素：setInterval(function(){$('div]').eq(i).GetTime('欢迎光临，今天是：','1');},1000); 
文本框：setInterval(function(){$('input').GetTime('','1','input')},1000);

=========================================================

Tab菜单切换 
 
HTML使用方法: 
<div dsh="tab" event="click"> 
     <div switchtab>      
           <a tab>a</a>        
           <a tab>b</a>      
           <a tab>c</a>     
     </div>    
     <div switchblock>      
           <p block>a</p>      
           <p block>b</p>    
           <p block>c</p>   
     </div>  
  </div>
   
 JS使用方法 
 $('div').tab('切换菜单标签','菜单选中样式','被切换标签容器','被切换标签','事件：click/hover');
 
 ======================================================
 
 创建在线QQ 
 
HTML使用方法:
 <em dsh="qq" qq="1594125370,1"></em>  
 <em dsh="qq" qq="1594125370,2"></em>  
 <em dsh="qq" qq="1594125370,3"></em>  
 <em dsh="qq" qq="1594125370,4"></em>  
 <em dsh="qq" qq="1594125370,5"></em>  
 <em dsh="qq" qq="1594125370,6"></em> 
  
 JS使用方法 
 $('div,p,li,span...').qq('QQ号','样式编号（1-17，41-50）');
 
 =======================================================
 
 获取URL中的参数值 
 
JS使用方法 
RequestQueryString['i'];

========================================================

左右无缝滚动 
 
HTML使用方法: 
<div dsh="roll">  
    <img src="Images/test.jpg" width="60" />  
    <img src="Images/test.jpg" width="60" />  
    <img src="Images/test.jpg" width="60" />  
    <img src="Images/test.jpg" width="60" />  
</div> 
 
JS使用方法 
$('div,p,li,span...').roll();

======================================================

滚屏效果上下（带控制）
  
HTML使用方法: 
<div dsh="rollTop" line="4" speed="200" timer="3000">  
    <div btnt>上上上</div>  
    <div roll style="height:100px; overflow:hidden;">  
        <ul>  
            <li>从前有坐山，山有有坐庙，庙里有个插件。</li>  ...  
        </ul>  
    </div>  
    <div btnb>下下下</div>  
</div> 
 
JS使用方法 
$('div,p,li,span...').rollTop({line:滚动行数,speed:速度,timer:时间间隔,up:"上按钮",down:"下按钮"});  
$('div,p,li,span...').rollTop({line:滚动行数,speed:速度,timer:时间间隔});

========================================================

滚屏效果（滚屏效果左右（带控制））
 
 HTML使用方法: 
 <div dsh="rollLeft" RollRow="滚动列数" DisplayRow="显示列数" SwitchBigImg="大图切换（*[bigImgObj]）不需要（false）" Title="大图切换标题（*[bigtitle]）不需要（false）" Time="自动滚动间隔时间为0则不自动滚动">
   <!--注意：SwitchBigImg和Title属性为大图元素和大图标题元素，如果不需要大图切换将其值写为false-->
       <div class="bigimg">  <img bigImgObj width="300" height="200">//不需要时直接去掉即可
           <p bigtitle>标题<;/p>//不需要时直接去掉即可
       </div>
       <div class="list">
          <div class="bn bnl" btnl>左</div>
          <div class="bn bnr" btnr>右</div>
          <div class="roll" roll>
                <ul>
                      <li title="标题一"><img src="Images/TestImg/01.jpg" bigSrc="Images/TestImg/01.jpg">标题一</li>
                      <li title="标题二"><img src="Images/TestImg/02.jpg" bigSrc="Images/TestImg/02.jpg">标题二</li>
                      <li title="标题三"><img src="Images/TestImg/03.jpg" bigSrc="Images/TestImg/03.jpg">标题三</li>
                      <li title="标题四"><img src="Images/TestImg/04.jpg" bigSrc="Images/TestImg/04.jpg">标题四</li>
                      <li title="标题五"><img src="Images/TestImg/05.jpg" bigSrc="Images/TestImg/05.jpg">标题五</li>
                      <li title="标题六"><img src="Images/TestImg/06.jpg" bigSrc="Images/TestImg/06.jpg">标题六</li>
                </ul>
           </div>
       </div>
  </div> 
                                                                     
JS使用方法 
$('滚动层').rollLeft({RollRow:滚动列数,DisplayRow:显示列数,Left:'左按钮',Right:'右按钮',Time:自动滚动间隔时间为0则不自动滚动,SwitchBigImg:'切换的大图对象',Title:'切换的标题对象'});

======================================================

简易提示层 
 
JS使用方法 
$.topPrompt(宽,高,'提示内容');

======================================================

插入flash 
 
HTML使用方法: 
<img src="..." dsh="imgAuto" maxWidth="80" ></li>  
 
JS使用方法 
$('div,p,li,span...').flash({src:'路径',width:'宽度',height:'高度',wmode:'显示模式（transparent）',mask:是否开启遮罩（true/flase）});

======================================================

操作Cookie 
 
JS使用方法 
写入：$.cookie('name','content'); 
读取：$.cookie('name');

======================================================

智能浮动层 
 
HTML使用方法: 
<div dsh="smartFloat">往上滚动，看我会怎样。</div> 
  
JS使用方法 
$('div,p,li,span...').smartFloat();

=====================================================

页面滚动图片等元素动态加载 
 
HTML使用方法: 
<img class="scrollLoading" data-url="图片真实地址" src="1*1gif图片" />  
 
JS使用方法 
$('div,p,li,span...').scrollLoading();

====================================================

事件的延时处理 
 
JS使用方法 
$('div,p,li,span...').hoverDelay({
   hoverDuring:500,//鼠标移上延时设置
   outDuring: 500,//鼠标移出延时设置
   hoverEvent: function(){
      alert("鼠标移上时执行的事件！");
   }
   outEvent: function(){
      alert("鼠标移出时执行的事件！"); 
    }  
  });
  
  ================================================
  
  静态分页 
 
HTML使用方法: 
<div dsh="pager" tag="li">
  <ul>
    <li>从前有坐山，山有有坐庙，庙里有个插件。</li>  ...  
  </ul>
</div> 
 
JS使用方法 
$('div').pager('分页标记',{
     navId: 'nav',//分页层Id
     navClass: 'Page',//分页层Class  
     navAttach: 'append',//添加分页方式 
     highlightClass: 'focus',//选中页样式 
     prevText: 'pre',//上一页文本 
     nextText: 'next',//下一页文本 
     height: null//分页层高度  
 });
 
 ===============================================
 
 向下翻页滚屏 
 
HTML使用方法: 
<div dsh="downpage">  
    <ul>
      <li>从前有坐山，山有有坐庙，庙里有个插件。</li>  ...  
    </ul>  
</div> 
 
JS使用方法 
$('div,p,li,span...').downpage({
  ButtonHtml:'',//设置翻页按钮内容 
  left:'',//按钮左定位 
  top:'',//按钮上定位 
  right:'',//按钮右定位 
  bottom:''//按钮下定位 
 });
 
 ==============================================
 
 创建随机验证码 
 
HTML使用方法: 
<div dsh="Code"></div>  
 
JS使用方法 
$('div,p,li,span...').Code();

===============================================

根随滚动 
 
HTML使用方法: 
<div dsh="Rscroll" top="-200" right="0">
    我不想呆在自己的坐位上。
</div>  
 
JS使用方法 
$('div,p,li,span...').Rscroll({top:上边距,left:左边距,right:右边距});

==============================================

下拉菜单跳转链接
  
HTML使用方法: 
<select dsh="jump">
      <option value="http://www.baidu.com">百度</option>      
      <option value="http://www.qq.com">腾讯</option>      
      <option value="http://www.taobao.com">淘宝</option>  
</select>

