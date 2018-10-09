<template>
    <div class="wrap">
        <!-- kv-->
        <section class="index">
            <div class="main">
                <div class="tt wow zoomInUp" data-wow-duration="1.2s">
                    <div class="fan">
                        <div class="fan_pos"><img src="../img/fan.png" alt=""></div>
                    </div>
                    <div class="ttBox"><img class="pc_dis" src="../img/tt.png" alt=""><img class="m_dis" src="../img/tt_m.png" alt=""></div>
                </div>
                <div class="leftOuter">
                    <div class="left wow zoomInLeft" data-wow-delay=".5s" data-wow-duration="1s"><img src="../img/line-l.png" alt=""></div>
                </div>
                <div class="rightOuter">
                    <div class="right wow zoomInRight" data-wow-delay=".5s" data-wow-duration="1s"><img src="../img/line-r.png" alt=""></div>
                </div>
            </div>
            <div class="bg"><img class="pc_dis" src="../img/city.png" alt=""><img class="m_dis" src="../img/city_m.png" alt=""></div>
            <div class="proOuter">
                <div class="pro_line wow zoomInUp" data-wow-delay="1s" data-wow-duration="1s"><img class="pc_dis" src="../img/pro-line.png" alt=""><img class="m_dis" src="../img/pro_line_m.png" alt=""></div>
            </div>
        </section>
        <!--intro-->
        <section class="intro">
            <div class="left">
                <div class="main">
                    <div class="wow fadeInUp" data-wow-offset="50">
                        <h3> <span class="icon"> <img src="../asset/svg/icon-company.svg" alt=""></span><span>企業介紹</span></h3>
                        <h2>領導廠商創新優勢</h2>
                        <p>台達電子是全球電源管理及散熱解決方案領導廠商，<span class="break">秉持「環保　節能　愛地球」的經營使命，</span><span class="break">運用電力電子核心技術，深耕台灣市場。</span></p>
                        <p>為因應工業4.0來臨，<span class="break">台達專注發展工業自動化產品和解決方案，</span><span class="break">同時積極開發智能機台、整合管理平台，</span><span class="break">建構智能製造系統與彈性多工智能產線。</span></p>
                        <p>台達積極發展品牌，營運據點遍佈全球，提供海外發展機會，<span class="break">熱情募集擁有創新思維人才，共創智能未來。</span></p>
                    </div>
                </div>
            </div>
            <div class="right wow fadeInUp" data-wow-offset="100"></div>
        </section>
        <!--worker-->
        <wrap-worker></wrap-worker>
        <!--learning-->
        <a class="apply_btn js-monitor-params" href="" @click="interBtn($event);"><span class="icon"><img src="../asset/svg/icon-apply.svg" alt=""></span><span>立即應徵</span></a>
        <section class="learning">
            <div class="wow fadeInUp">
                <div class="tt">
                    <h3> <span class="icon"> <img src="../asset/svg/icon-book.svg" alt=""></span><span>學習發展</span></h3>
                    <h2>循序漸進訓練發展</h2>
                </div>
                <div class="chart"><img class="pc_dis" src="../asset/svg/chart.svg" alt=""><img class="m_dis" src="../asset/svg/chart_m.svg" alt=""></div>
                <div class="culture">
                    <ul>
                        <li>實務訓練</li>
                        <li>策略發展</li>
                        <li>願景領導</li>
                    </ul>
                    <div class="sub">文化塑型</div>
                </div>
                <div class="dot_bg"></div>
            </div>
        </section>
        <!--welfare-->
        <section class="welfare">
            <div class="tt wow fadeInUp">
                <h3> <span class="icon"> <img src="../asset/svg/icon-like.svg" alt=""></span><span>優質福利</span></h3>
                <h2>多元完善優質福利</h2>
            </div>
            <div class="main">
                <div class="box wow fadeInUp">
                    <div class="tt">多元完善優質福利</div>
                    <ul>
                        <li>年薪上看<span>20個月</span></li>
                        <li>旅遊補助<span>$10,000元</span></li>
                        <li>生日禮券及蛋糕</li>
                        <li>黃金旅遊假(有薪)</li>
                        <li>員工健檢方案</li>
                        <li>員工團體保險(公費含子女及配偶)</li>
                        <li>員工餐廳月付500元<span>享三餐</span></li>
                    </ul>
                </div>
                <div class="box wow fadeInUp">
                    <div class="tt">員工個人發展接軌國際</div>
                    <ul>
                        <li> <span>全額補助</span>外部技術研討及技能訓練</li>
                        <li>全球64個研發中心進階學習</li>
                        <li>e-Learning學習平台</li>
                        <li>管理與技術職<span>雙軌晉升</span></li>
                        <li> <span>放眼全球</span>的工作歷練及發展</li>
                        <li>參與國際知名專家主持專案</li>
                    </ul>
                </div>
            </div>
            <div class="picBox">
                <div class="pic wow fadeInUp" data-wow-delay=".2s"><img src="../img/p1.jpg" alt=""></div>
                <div class="pic wow fadeInUp" data-wow-delay=".3s"><img src="../img/p2.jpg" alt=""></div>
                <div class="pic wow fadeInUp" data-wow-delay=".4s"><img src="../img/p3.jpg" alt=""></div>
            </div>
            <div class="deco1"><img src="../img/deco2.png" alt=""></div>
            <div class="deco2"><img src="../img/deco1.png" alt=""></div>
        </section>
    </div>
</template>

<script>
    import content from './wrapworker.vue';
    export default {
        name: 'wrap',
        data () {
            return {
                
            }
        },
        components:{
            'wrap-worker': content
        },
        created: function () {
            window.addEventListener('scroll', this.scroll);
        },
        mounted: function(){
            this.initWow();
        },
        methods: {
            initWow: function(){
                var wowArr = document.querySelectorAll('.worker .main, .worker .job h2, .worker .job .container, .worker .job .btn, .worker .job .mt, .worker .job .solar_box');
                for(var i = 0; i < wowArr.length; i++) {
                    wowArr[i].classList.add('wow');
                    wowArr[i].classList.add('fadeInUp');
                    wowArr[i].setAttribute('data-wow-offset', '50');
                }
            },
            interBtn: function(evt){
                evt.preventDefault();
                var pos = document.querySelector('.worker').offsetTop;
                this.$parent.scrollToY(pos, 500);
            },
            scroll: function(){
                var disTop = window.scrollY;
                var learnTop = document.querySelector('.learning').offsetTop - document.querySelector('.learning').offsetHeight;
                var ctrlObj = document.querySelector('.apply_btn');
                if(disTop > learnTop){
                    ctrlObj.classList.add('show');
                }else{
                    ctrlObj.classList.remove('show');
                }
            }
        },
        destroyed: function () {
            window.removeEventListener('scroll', this.scroll);
        }
    }
</script>

<style>
    .apply_btn{
        display: block;
        visibility: hidden; 
        opacity: 0;
    }
    .apply_btn.show{
        opacity: 1;
        visibility: visible; 
    }
</style>