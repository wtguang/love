跳到内容
 
Search or jump to…

拉请求
问题
市场
探索
 
@wtguang 
0
0 0 wtguang / 爱
 代码 问题0 拉取请求0 项目 0 Wiki Insights 设置   
love /Love.html
@wtguang wtguang 修改
47ff210
4分钟前
221线（196 sloc）  8.89 KB
    
<！DOCTYPE html PUBLIC “ -  // W3C // DTD XHTML 1.0 Strict // EN”  “http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd” >
<！ -保存自url =（0027）http://itzoo.info/love.html - >
< html  xml：lang = “ en ”  xmlns = “ http://www.w3.org/1999/xhtml ” > < head > < meta  http-equiv = “ Content-Type ”  content = “ text / html; charset = UTF-8 “ >
        < title >爱</ title >
        
        < link  type = “ text / css ”  rel = “ stylesheet ”  href = “ ./ Love_files/default.css ” >
        < script  type = “ text / javascript ”  src = “。/ Love_files / jquery.min.js ” > </ script >
        < script  type = “ text / javascript ”  src = “ ./ Love_files / jscex.min.js ” > </ script >
        < script  type = “ text / javascript ”  src = “ ./ Love_files / jscex-parser.js ” > </ script >
        < script  type = “ text / javascript ”  src = “ ./ Love_files / jscex-jit.js ” > </ script >
        < script  type = “ text / javascript ”  src = “ ./ Love_files / jscex-builderbase.min.js ” > </ script >
        < script  type = “ text / javascript ”  src = “ ./ Love_files / jscex-async.min.js ” > </ script >
        < script  type = “ text / javascript ”  src = “ ./ Love_files / jscex-async-powerpack.min.js ” > </ script >
        < 脚本 类型 = “文本/ JavaScript的”  SRC = “ ./Love_files/functions.js ” 字符集 = “ UTF-8 ” > </ 脚本 >
        < script  type = “ text / javascript ”  src = “。/ Love_files  / love.js ” charset = “ utf-8 ” > </ script >

    </ head >
    < body >
        < div  id = “ main ” >
            < div  id = “ error ” >亲，您使用的浏览器无法支持即将显示的内容，请换成谷歌（< a  href = “ http://www.google.cn/chrome/intl/zh-CN/ landing_chrome.html？HL = ZH-CN＆品牌= CHMI “ >铬</ 一 >）或者火狐（< 一个 HREF = ” http://firefox.com.cn/download/ “ >火狐</ 一 >）浏览器哟〜</ div >
            < div  id = “ wrap ” >
               < div  id = “ text ” >
                    < div  id = “ code ” >                 
                    < 跨度 类 = “说” >我的爱人，我会牵着你的手，走到满头白发的那一天，</ 跨度 > < BR >
                    < 跨度 类 = “说” >我会守护你生命里的精彩，并陪伴你一路精彩下去。</ 跨度 > < BR >
                    < 跨度 类 = “说” >你的幸福快乐，是我一生的追求。</ 跨度 > < BR >
                    < 跨度 类 = “说” >我会每一天带着笑脸，和你说早安，</ 跨度 > < BR >
                     < 跨度 类 = “说” >我会每一晚与你道声晚安再入梦乡，</ 跨度 > < BR >
                    < 跨度 类 = “说” >我会带你去所有你想去的地方，</ 跨度 > < BR >
                    < 跨度 类 = “说” >陪你闹看你笑</ 跨越 > < BR >
                    < 跨度 类 = “说” >历经你生命中所有的点点滴滴。</ 跨度 > < BR >
                    < 跨度 类 = “说” >我期待这一生与你一起走过，</ 跨度 > < BR >
                    < 跨度 类 = “说” >我期待与你慢慢变老</ 跨越 > < BR >
                    < 跨度 类 = “说” >等我们老到哪儿也去不了，</ 跨度 > < BR >
                    < 跨度 类 = “说” >还能满载着一生的幸福快乐！</ 跨度 > < BR >
                    < BR >
                    < 跨度 类 = “说” >我会为我们的未来撑起一片天空，</ 跨度 > < BR >
                     < 跨度 类 = “说” >为我们的将来担负起一生的责任，</ 跨度 > < BR >
                      < 跨度 类 = “说” >愿意为你去做每一件能让你开心快乐的事。</ 跨度 > < BR >
                       < 跨度 类 = “说” >所有我们经历的点点滴滴，</ 跨度 > < BR >
                        < 跨度 类 = “说” >都是我们一辈子最美的回忆。</ 跨度 > < BR >
                         < 跨度 类 = “说” >我愿意爱你直到老去！</ 跨度 > < BR >
                   < BR >
                    < span  class = “ say ” > < span  class = “ space ” > </ span >  - 你的，宝宝。</ span >
                    </ div >
                </ div >
                <div id="clock-box">
                    <a href="http://blog.csdn.net/wuxia2001" target="_blank">我</a> 与 <a href="http://blog.csdn.net/wuxia2001" target="_blank">大宝贝儿</a> 在一起的
                        <div id="clock"></div>
                </div>
                <canvas id="canvas" width="1100" height="680"></canvas>
            </div>
            <audio src="love.mp3" autoplay="autoplay"></audio>
        </div>
    
    <script>
    </script>

    <script>
    (function(){
        var canvas = $('#canvas');
        if (!canvas[0].getContext) {
            $("#error").show();
            return false;
        }
        var width = canvas.width();
        var height = canvas.height();
        
        canvas.attr("width", width);
        canvas.attr("height", height);
        var opts = {
            seed: {
                x: width / 2 - 20,
                color: "rgb(190, 26, 37)",
                scale: 2
            },
            branch: [
                [535, 680, 570, 250, 500, 200, 30, 100, [
                    [540, 500, 455, 417, 340, 400, 13, 100, [
                        [450, 435, 434, 430, 394, 395, 2, 40]
                    ]],
                    [550, 445, 600, 356, 680, 345, 12, 100, [
                        [578, 400, 648, 409, 661, 426, 3, 80]
                    ]],
                    [539, 281, 537, 248, 534, 217, 3, 40],
                    [546, 397, 413, 247, 328, 244, 9, 80, [
                        [427, 286, 383, 253, 371, 205, 2, 40],
                        [498, 345, 435, 315, 395, 330, 4, 60]
                    ]],
                    [546, 357, 608, 252, 678, 221, 6, 100, [
                        [590, 293, 646, 277, 648, 271, 2, 80]
                    ]]
                ]] 
            ],
            bloom: {
                num: 700,
                width: 1080,
                height: 650,
            },
            footer: {
                width: 1200,
                height: 5,
                speed: 10,
            }
        }
        var tree = new Tree(canvas[0], width, height, opts);
        var seed = tree.seed;
        var foot = tree.footer;
        var hold = 1;
        canvas.click(function(e) {
            var offset = canvas.offset(), x, y;
            x = e.pageX - offset.left;
            y = e.pageY - offset.top;
            if (seed.hover(x, y)) {
                hold = 0; 
                canvas.unbind("click");
                canvas.unbind("mousemove");
                canvas.removeClass('hand');
            }
        }).mousemove(function(e){
            var offset = canvas.offset(), x, y;
            x = e.pageX - offset.left;
            y = e.pageY - offset.top;
            canvas.toggleClass('hand', seed.hover(x, y));
        });
        var seedAnimate = eval(Jscex.compile("async", function () {
            seed.draw();
            while (hold) {
                $await(Jscex.Async.sleep(10));
            }
            while (seed.canScale()) {
                seed.scale(0.95);
                $await(Jscex.Async.sleep(10));
            }
            while (seed.canMove()) {
                seed.move(0, 2);
                foot.draw();
                $await(Jscex.Async.sleep(10));
            }
        }));
        var growAnimate = eval(Jscex.compile("async", function () {
            do {
                tree.grow();
                $await(Jscex.Async.sleep(10));
            } while (tree.canGrow());
        }));
        var flowAnimate = eval(Jscex.compile("async", function () {
            do {
                tree.flower(2);
                $await(Jscex.Async.sleep(10));
            } while (tree.canFlower());
        }));
        var moveAnimate = eval(Jscex.compile("async", function () {
            tree.snapshot("p1", 240, 0, 610, 680);
            while (tree.move("p1", 500, 0)) {
                foot.draw();
                $await(Jscex.Async.sleep(10));
            }
            foot.draw();
            tree.snapshot("p2", 500, 0, 610, 680);
            // 会有闪烁不得意这样做, (＞﹏＜)
            canvas.parent().css("background", "url(" + tree.toDataURL('image/png') + ")");
            canvas.css("background", "#ffe");
            $await(Jscex.Async.sleep(300));
            canvas.css("background", "none");
        }));
        var jumpAnimate = eval(Jscex.compile("async", function () {
            var ctx = tree.ctx;
            while (true) {
                tree.ctx.clearRect(0, 0, width, height);
                tree.jump();
                foot.draw();
                $await(Jscex.Async.sleep(25));
            }
        }));
        var textAnimate = eval(Jscex.compile("async", function () {
            var together = new Date();
            together.setFullYear(2017, 10, 12);
            together.setHours(13);
            together.setMinutes(14);
            together.setSeconds(52);
            together.setMilliseconds(0);
            $("#code").show().typewriter();
            $("#clock-box").fadeIn(500);
            while (true) {
                timeElapse(together);
                $await(Jscex.Async.sleep(1000));
            }
        }));
        VAR runAsync =  EVAL（Jscex。编译（“异步”，函数（）{
            $ await（seedAnimate（））;
            $ await（growAnimate（））;
            $ await（flowAnimate（））;
            $ await（moveAnimate（））;
            textAnimate（）。start（）;
            $ await（jumpAnimate（））;
        }））;
        runAsync（）。start（）;
    }）（）;
    </ script >



</ body > </ html >
©2019 GitHub，Inc。
条款
隐私
安全
状态
救命
联系GitHub
价钱
API
训练
博客
关于
