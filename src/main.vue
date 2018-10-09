<template>
    <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0">
        <tr>
            <td>
                <table width="100%" border="0" cellspacing="0" cellpadding="0">
                    <!-- Header 表頭 -->
                    <tr>
                        <td>
                            <table width="100%" border="0" cellspacing="0" cellpadding="0">
                                <tr style="font-size: 12px;color: #333333;line-height: 22px;">
                                    <td>
                                        <table width="100%" border="0" cellspacing="0" cellpadding="0">
                                            <tr>
                                                <td width="141"><img src="http://www.104.com.tw/cfdocs/edm/mutual_img/edm_logo2.jpg" width="141" height="32" /></td>
                                                <td align="right">→以下是台達電子提供的內容</td>
                                            </tr>
                                        </table>
                                    </td>
                                </tr>
                            </table>
                        </td>
                    </tr>
                    <!-- Content 內容 -->
                    <tr>
                        <td>
                            <div class="body">
                                <trans-bg></trans-bg>
                                <menu-nav></menu-nav>
                                <wrap-content></wrap-content>
                                <!-- 廣告追蹤機制 
                                <script type="text/javascript" src="//static.104.com.tw/104main/js/common/monitorParm.js "></script>-->
                            </div>
                        </td>
                    </tr>
                    <!-- Footer 表尾 -->
                    <tr>
                        <td height="100%" align="center" style="text-align: center;padding: 10px;"><span style="font:12px Arial;color:#333;letter-spacing:1px;line-height:22px;">上述內容由 台達電子 提供，104整合招募服務處代為維護管理<br />
                            以上所提及之各公司與產品均分屬各相關公司與個別擁有者之商標<br />
                            意見反應：02-29126104#8163 <a href="http://www.104.com.tw/cfdocs/question_admin/user/reaction.cfm" target="_blank" width="20px" style="display: inline-block;"><img src="http://www.104.com.tw/cfdocs/edm/mutual_img/edm_mail_im_01.gif" border="0" align="absmiddle"></a><br>
                            本網站內容享有著作權，禁止侵害，違者必究。&copy; 2001-2016 104 Corporation All Rights Reserved </span>
                        </td>
                    </tr>
                </table>
            </td>
        </tr>
    </table>
</template>

<script>
    import wow from 'wow.js';
    import transbg from './component/transbg.vue';
    import menu from './component/menu.vue';
    import wrap from './component/wrap.vue';
    window.requestAnimFrame = (function(){
      return  window.requestAnimationFrame       ||
              window.webkitRequestAnimationFrame ||
              window.mozRequestAnimationFrame    ||
              function( callback ){
                window.setTimeout(callback, 1000 / 60);
              };
    })();
    export default {
        name: 'main',
        data () {
            return {
                
            }
        },
        components:{
            'trans-bg': transbg,
            'menu-nav': menu,
            'wrap-content': wrap
        },
        mounted: function(){
            window.addEventListener('load', function(event) {
                new wow().init();
            });
        },
        methods: {
            // 共用function要放在父層templete
            scrollToY: function(scrollTargetY, speed, easing){
                // scrollTargetY: the target scrollY property of the window
                // speed: time in pixels per second
                // easing: easing equation to use

                var scrollY = window.scrollY || document.documentElement.scrollTop,
                    scrollTargetY = scrollTargetY || 0,
                    speed = speed || 2000,
                    easing = easing || 'easeOutSine',
                    currentTime = 0;

                // min time .1, max time .8 seconds
                var time = Math.max(.1, Math.min(Math.abs(scrollY - scrollTargetY) / speed, .8));

                // easing equations from https://github.com/danro/easing-js/blob/master/easing.js
                var easingEquations = {
                        easeOutSine: function (pos) {
                            return Math.sin(pos * (Math.PI / 2));
                        },
                        easeInOutSine: function (pos) {
                            return (-0.5 * (Math.cos(Math.PI * pos) - 1));
                        },
                        easeInOutQuint: function (pos) {
                            if ((pos /= 0.5) < 1) {
                                return 0.5 * Math.pow(pos, 5);
                            }
                            return 0.5 * (Math.pow((pos - 2), 5) + 2);
                        }
                    };

                // add animation loop
                function tick() {
                    currentTime += 1 / 60;
                    var p = currentTime / time;
                    var t = easingEquations[easing](p);

                    if (p < 1) {
                        requestAnimFrame(tick);
                        window.scrollTo(0, scrollY + ((scrollTargetY - scrollY) * t));
                    } else {
                        window.scrollTo(0, scrollTargetY);
                    }
                }

                // call it once to get started
                tick();
            }
        }
    }
</script>

<style>
    @import './static/style.css';
    @import './static/animate.min.css';
    .wow{
        visibility: hidden;
    }
</style>
