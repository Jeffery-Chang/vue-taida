<template ref="menu">
    <section class="worker">
        <div class="wow fadeInUp" data-wow-offset="50">
            <div class="tt">
                <h3> <span class="icon"> <img src="../asset/svg/icon-star.svg" alt=""></span><span>智能人才</span></h3>
                <h2>智能人才實踐想像</h2>
                <p class="spec"> <span class="large">台達</span>能給你比想像的更多</p>
                <p>台達擁有豐富的資源及能力，讓人才發揮自身所長！<span class="break">智能人才能在這裡，得以實現理想，並讓自己走在世界的前端。</span></p>
            </div>
        </div>
        <div class="deco"><img src="../img/deco3.png" alt=""></div>
        <!--tab-->
        <div class="wow fadeInUp" data-wow-offset="100">
            <div class="tab">
                <ul>
                    <li @click="hashSet($event, '1');"><a :class="{ 'active' : (hash == '1') }" href="#hash1">機構設計</a></li>
                    <li @click="hashSet($event, '2');"><a :class="{ 'active' : (hash == '2') }" href="#hash2">FAE</a></li>
                    <li @click="hashSet($event, '3');"><a :class="{ 'active' : (hash == '3') }" href="#hash3">機械設計</a></li>
                    <li @click="hashSet($event, '4');"><a :class="{ 'active' : (hash == '4') }" href="#hash4">軟體開發</a></li>
                    <li @click="hashSet($event, '5');"><a :class="{ 'active' : (hash == '5') }" href="#hash5">軟體設計</a></li>
                </ul>
            </div>
        </div>
        <div class="p1" v-show="hash == '1'">
            <div class="main">
                <div class="ppl">
                    <div class="pic_pos">
                        <div class="inner">
                            <div class="pic">
                                <div class="inner">
                                    <div class="num"><img src="../asset/svg/01.svg" alt=""></div>
                                    <div class="name">
                                        <div class="inner">
                                            <ul>
                                                <li><img src="../asset/svg/icon-target.svg" alt=""></li>
                                                <li>丁必陞</li>
                                                <li>機構設計資深工程師</li>
                                                <li>年資1年</li>
                                            </ul>
                                        </div>
                                    </div><img class="pc_dis" src="../img/PPL1.png" alt=""><img class="m_dis" src="../img/PPL1_m.png" alt="">
                                </div>
                            </div>
                            <div class="bg"><img src="../img/deco4.png" alt=""></div>
                        </div>
                    </div>
                </div>
                <!--txt-->
                <div class="content">
                    <h4>選擇台達的原因</h4>
                    <p>個人能在台達獲得專業上的成就。另外，台達的產品定位明確及全球化程度相當高，希望自己能為這樣的產品出一份力。</p>
                    <h4>在台達的成長</h4>
                    <ul>
                        <li>藉由公司內外部的訓練，能讓我在產品設計上能夠更加全面。</li>
                        <li>在跨部門的協助當中，必須考量到對方的想法，從中找到更好的解決方案，使得自己在做事上更圓融。</li>
                    </ul>
                    <h4>建議應徵此職務必備技能</h4>
                    <p>除了基本的機械常識外，首先必須要有良好的溝通能力，因為除了設計之外必須跟客戶、廠商、部門之間進行溝通，才能讓你的產品(設備)更加完善。接著，還必須要有良好的規劃能力，不管是在時間管控及專案執行上，都必須要有完善的規劃能力。</p>
                    <h4>給新鮮人的一句話</h4>
                    <h5> <span class="txt">相信自己的選擇<span class="d1"><img src="../asset/svg/d1.svg" alt=""></span><span class="d2"> <img src="../asset/svg/d2.svg" alt=""></span></span></h5>
                </div>
                <div class="dot_bg"></div>
                <div class="ppl_bg"><img src="../img/PPL1-2.png" alt=""></div>
            </div>
            <div class="job">
                <h2>自動化機械設計工程師(中壢)</h2>
                <div class="container">
                    <div class="left">
                        <div class="box">
                            <div class="tt">工作內容</div>
                            <ul>
                                <li>執行市場產品(自動化機械)趨勢研究</li>
                                <li>機構設計類零部件結構/功能設計的執行</li>
                                <li>機構設計類產品設計input/output審查的執行</li>
                                <li>機構設計類產品BOM手稿提供與確認的規劃與執行</li>
                                <li>規劃與執行機構設計類零件材料選用及供應商導入</li>
                                <li>擬定與執行機構設計類工程/設計變更</li>
                            </ul>
                        </div>
                    </div>
                    <div class="right">
                        <div class="box">
                            <div class="tt">需求年資與背景</div>
                            <ul>
                                <li>碩士畢業，2年以上經驗</li>
                                <li>機械工程相關系所畢業</li>
                            </ul>
                        </div>
                        <div class="box">
                            <div class="tt">具備技能</div>
                            <p>熟悉使用Auto-CAD、PRO/E</p>
                        </div>
                    </div>
                </div><a class="btn js-monitor-params" href="https://www.104.com.tw/job/?jobno=3uve9" target="_blank"><span>立即應徵</span><span class="icon"> <img src="../asset/svg/arrow.svg" alt=""></span></a>
                <div class="mt"><img src="../img/mt.png" alt=""></div>
                <div class="solar_box">
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                </div>
            </div>
        </div>
        <div class="p2" v-show="hash == '2'">
            <div class="main">
                <div class="ppl">
                    <div class="pic_pos">
                        <div class="inner">
                            <div class="pic">
                                <div class="inner">
                                    <div class="num"><img src="../asset/svg/02.svg" alt=""></div>
                                    <div class="name">
                                        <div class="inner">
                                            <ul>
                                                <li><img src="../asset/svg/icon-target.svg" alt=""></li>
                                                <li>何昌明</li>
                                                <li>FAE資深課長</li>
                                                <li>年資7.8年</li>
                                            </ul>
                                        </div>
                                    </div><img class="pc_dis" src="../img/PPL2.png" alt=""><img class="m_dis" src="../img/PPL2_m.png" alt="">
                                </div>
                            </div>
                            <div class="bg"><img src="../img/deco4.png" alt=""></div>
                        </div>
                    </div>
                </div>
                <!--txt-->
                <div class="content">
                    <h4>選擇台達的原因</h4>
                    <p>當初因欣賞創辦人鄭先生的經營理念而進入台達。台達體系完整、穩定成長，且機電事業群擁有完整的工業自動化產品，從設備層、控制層、到最上位的資訊層，可提供客戶整套解決方案，引領業界邁向工業4.0智慧製造之路。</p>
                    <h4>在台達的成長</h4>
                    <p>台達擁有完整的培訓制度，個人由一開始的FAE工程師，到如今擔任管理職，公司在不同職務位置會提供員工相對應的訓練課程，讓員工持續成長茁壯。</p>
                    <h4>建議應徵此職務必備技能</h4>
                    <p>電機/機械相關科系畢業，熟悉工控產品，擁有自動化相關經驗。</p>
                    <h4>給新鮮人的一句話</h4>
                    <h5> <span class="txt">電機/機械相關科系畢業，熟悉工控產品，擁有自動化相關經驗。<span class="d1"><img src="../asset/svg/d1.svg" alt=""></span><span class="d2"> <img src="../asset/svg/d2.svg" alt=""></span></span></h5>
                </div>
                <div class="dot_bg"></div>
                <div class="ppl_bg"><img src="../img/PPL2-2.png" alt=""></div>
            </div>
            <div class="job">
                <h2>FAE應用工程師(智能訊息)<br>智慧感測器事業處IABG(桃園三廠)</h2>
                <div class="container">
                    <div class="left">
                        <div class="box">
                            <div class="tt">工作內容</div>
                            <ul>
                                <li>工控產品應用整合技術服務</li>
                                <li>新產品、新行業市場推廣</li>
                                <li>產品操作說明文件製作</li>
                                <li>應用案例文件製作</li>
                                <li>擔任培訓講師，進行常規產品培訓</li>
                                <li>協助業務處理客戶問題</li>
                                <li>提供客戶正確的產品規格與應用整合服務</li>
                                <li>協助客戶端現場試機與售前售後技術服務</li>
                            </ul>
                        </div>
                    </div>
                    <div class="right">
                        <div class="box">
                            <div class="tt">需求年資與背景</div>
                            <ul>
                                <li>碩士畢業，2年以上經驗</li>
                                <li>電機電子、機械工程、自動控制、其他工程相關系所畢業</li>
                            </ul>
                        </div>
                        <div class="box">
                            <div class="tt">具備技能</div>
                            <ul>
                                <li>PLC產品開發經驗尤佳 </li>
                                <li>英文能力中等以上</li>
                                <li>具備機器視覺基礎知識</li>
                            </ul>
                        </div>
                    </div>
                </div><a class="btn js-monitor-params" href="https://www.104.com.tw/job/?jobno=5r6gd" target="_blank"><span>立即應徵</span><span class="icon"> <img src="../asset/svg/arrow.svg" alt=""></span></a>
                <div class="mt"><img src="../img/mt.png" alt=""></div>
                <div class="solar_box">
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                </div>
            </div>
        </div>
        <div class="p3" v-show="hash == '3'">
            <div class="main">
                <div class="ppl">
                    <div class="pic_pos">
                        <div class="inner">
                            <div class="pic">
                                <div class="inner">
                                    <div class="num"><img src="../asset/svg/03.svg" alt=""></div>
                                    <div class="name">
                                        <div class="inner">
                                            <ul>
                                                <li><img src="../asset/svg/icon-target.svg" alt=""></li>
                                                <li>李佩君</li>
                                                <li>機械設計資深課長</li>
                                                <li>年資5年</li>
                                            </ul>
                                        </div>
                                    </div><img class="pc_dis" src="../img/PPL3.png" alt=""><img class="m_dis" src="../img/PPL3_m.png" alt="">
                                </div>
                            </div>
                            <div class="bg"><img src="../img/deco4.png" alt=""></div>
                        </div>
                    </div>
                </div>
                <!--txt-->
                <div class="content">
                    <h4>選擇台達的原因</h4>
                    <p>由於自動化的發展是逐步被重視的，機器人產業勢必成為主流產品，得知台達要成立機器人部門時，就立即選擇加入台達。</p>
                    <h4>在台達的成長</h4>
                    <ul>
                        <li>每月都有多場專業能力提升課程，也有線上語言進修課程。</li>
                        <li>參加國內外展覽活動，充實個人視野及增加產品設計靈感。</li>
                        <li>針對管理職會有專業講師，加強工作效率提升、專案管理。</li>
                    </ul>
                    <h4>建議應徵此職務必備技能</h4>
                    <p>專業能力是基本的條件，另外就是個人的熱忱及態度。</p>
                    <h4>給新鮮人的一句話</h4>
                    <h5> <span class="txt">勇於嘗試，挑戰自我<span class="d1"><img src="../asset/svg/d1.svg" alt=""></span><span class="d2"> <img src="../asset/svg/d2.svg" alt=""></span></span></h5>
                </div>
                <div class="dot_bg"></div>
                <div class="ppl_bg"><img src="../img/PPL3-2.png" alt=""></div>
            </div>
            <div class="job">
                <h2>機構設計工程師_台中分公司(中科)</h2>
                <div class="container">
                    <div class="left">
                        <div class="box">
                            <div class="tt">工作內容</div>
                            <ul>
                                <li>自動化設備機構設計、測試、導入</li>
                                <li>自動化應用產品機構設計、測試</li>
                                <li>智慧型機器人設計、測試</li>
                            </ul>
                        </div>
                    </div>
                    <div class="right">
                        <div class="box">
                            <div class="tt">需求年資與背景</div>
                            <ul>
                                <li>碩士畢業，2年以上經驗</li>
                                <li>電機電子工程、機械工程、自動控制、其他工程相關系所畢業</li>
                            </ul>
                        </div>
                        <div class="box">
                            <div class="tt">具備技能</div>
                            <ul>
                                <li>具3D CAD、 Inventer工具設計經驗者尤佳</li>
                                <li>具自動化設備機構設計開發經驗者尤佳</li>
                            </ul>
                        </div>
                    </div>
                </div><a class="btn js-monitor-params" href="https://www.104.com.tw/job/?jobno=3xlmn" target="_blank"><span>立即應徵</span><span class="icon"> <img src="../asset/svg/arrow.svg" alt=""></span></a>
                <div class="mt"><img src="../img/mt.png" alt=""></div>
                <div class="solar_box">
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                </div>
            </div>
        </div>
        <div class="p4" v-show="hash == '4'">
            <div class="main">
                <div class="ppl">
                    <div class="pic_pos">
                        <div class="inner">
                            <div class="pic">
                                <div class="inner">
                                    <div class="num"><img src="../asset/svg/04.svg" alt=""></div>
                                    <div class="name">
                                        <div class="inner">
                                            <ul>
                                                <li><img src="../asset/svg/icon-target.svg" alt=""></li>
                                                <li>張嘉裕</li>
                                                <li>軟體設計資深工程師</li>
                                                <li>年資4年</li>
                                            </ul>
                                        </div>
                                    </div><img class="pc_dis" src="../img/PPL4.png" alt=""><img class="m_dis" src="../img/PPL4_m.png" alt="">
                                </div>
                            </div>
                            <div class="bg"><img src="../img/deco4.png" alt=""></div>
                        </div>
                    </div>
                </div>
                <!--txt-->
                <div class="content">
                    <h4>選擇台達的原因</h4>
                    <p>一開始是因為台達發展穩定及營收成長，所以選擇進入台達。再者因為自己研究與視覺演算法相關，而當時視覺演算法研究與開發類型的工作缺額並不多，因此能夠得到這份工作覺得相當開心。</p>
                    <h4>在台達的成長</h4>
                    <p>接觸更多之後會學習到軟體規劃與架構設計的重要，也有很多機會學習到不同的軟體套件與工具應用，這些可提升專業技能。
                        <br>個人也有國內外出差的機會，以工作層面來說，能直接了解客戶需求，也有機會窺探競爭對手的機器與技術，以個人層面來說，等於是有機會獨立旅行到不同地方去走走增廣見聞。</p>
                    <h4>建議應徵此職務必備技能</h4>
                    <ul>
                        <li>程式語言-具備撰寫程式語言的邏輯思維，若能熟練使用C/C++會是一大優勢。</li>
                        <li>研究能力-根據一個主題進行文獻探討、實現方法、改進方法及創新的過程。</li>
                        <li>團隊合作-適時與其他團隊成員相互討論、互相幫助，讓團隊達成共同目標。</li>
                        <li>追求新知的渴望與實事求是的態度。</li>
                    </ul>
                    <h4>給新鮮人的一句話</h4>
                    <h5> <span class="txt">程式語言只是工具，<span class="break">卻能撰寫出優美的詩詞來證明自己價值。</span><span class="d1"><img src="../asset/svg/d1.svg" alt=""></span><span class="d2"> <img src="../asset/svg/d2.svg" alt=""></span></span></h5>
                </div>
                <div class="dot_bg"></div>
                <div class="ppl_bg"><img src="../img/PPL4-2.png" alt=""></div>
            </div>
            <div class="job">
                <h2>軟體工程師(機器視覺)<br>智慧感測器事業處IABG(桃園三廠)</h2>
                <div class="container">
                    <div class="left">
                        <div class="box">
                            <div class="tt">工作內容</div>
                            <ul>
                                <li>機器視覺，影像處理，演算法開發</li>
                                <li>熟悉Machine Learning / Deep Learning</li>
                            </ul>
                        </div>
                    </div>
                    <div class="right">
                        <div class="box">
                            <div class="tt">需求年資與背景</div>
                            <ul>
                                <li>碩士畢業，2年以上經驗</li>
                                <li>電機電子、自動控制、資訊工程相關系所畢業</li>
                            </ul>
                        </div>
                        <div class="box">
                            <div class="tt">具備技能</div>
                            <p>熟悉使用C、C++、Matlab、Python</p>
                        </div>
                    </div>
                </div><a class="btn js-monitor-params" href="https://www.104.com.tw/job/?jobno=3vurs" target="_blank"><span>立即應徵</span><span class="icon"> <img src="../asset/svg/arrow.svg" alt=""></span></a>
                <div class="mt"><img src="../img/mt.png" alt=""></div>
                <div class="solar_box">
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                </div>
            </div>
        </div>
        <div class="p5" v-show="hash == '5'">
            <div class="main">
                <div class="ppl">
                    <div class="pic_pos">
                        <div class="inner">
                            <div class="pic">
                                <div class="inner">
                                    <div class="num"><img src="../asset/svg/05.svg" alt=""></div>
                                    <div class="name">
                                        <div class="inner">
                                            <ul>
                                                <li><img src="../asset/svg/icon-target.svg" alt=""></li>
                                                <li>許傑巽</li>
                                                <li>軟體設計資深工程師</li>
                                                <li>年資4年</li>
                                            </ul>
                                        </div>
                                    </div><img class="pc_dis" src="../img/PPL5.png" alt=""><img class="m_dis" src="../img/PPL5_m.png" alt="">
                                </div>
                            </div>
                            <div class="bg"><img src="../img/deco4.png" alt=""></div>
                        </div>
                    </div>
                </div>
                <!--txt-->
                <div class="content">
                    <h4>選擇台達的原因</h4>
                    <p>當初因為想從事機器人相關的領域，發現台達電有機器人部門且擁有許多資源，包括有自行研發馬達和研發機器視覺的能力，因此如果說台灣有誰有最豐富的資訊來做機械手臂的話，我覺得一定是台達。</p>
                    <h4>在台達的成長</h4>
                    <ul>
                        <li>因為機械手臂在使用上需進行許多模組的整合，因此有機會進行跨部門整合。</li>
                        <li>能第一線接觸到終端使用者，聽取使用者需求及意見。</li>
                        <li>常有機會參與國際性的展覽，除了可跟國外同事交流外，也能增加自己的國際視野。</li>
                    </ul>
                    <h4>建議應徵此職務必備技能</h4>
                    <p>電機、機械、資工相關科系畢業，熟悉線性代數，有一定的空間概念，有一定的編程能力。</p>
                    <h4>給新鮮人的一句話</h4>
                    <h5> <span class="txt">加入台達，飛黃騰達<span class="d1"><img src="../asset/svg/d1.svg" alt=""></span><span class="d2"> <img src="../asset/svg/d2.svg" alt=""></span></span></h5>
                </div>
                <div class="dot_bg"></div>
                <div class="ppl_bg"><img src="../img/PPL5-2.png" alt=""></div>
            </div>
            <div class="job">
                <h2>軟體設計工程師_台中分公司(中科)</h2>
                <div class="container">
                    <div class="left">
                        <div class="box">
                            <div class="tt">工作內容</div>
                            <ul>
                                <li>機器人操作軟體開發，建立友善的操作介面</li>
                                <li>整合/應用第三方軟件，加速軟體開發時程</li>
                                <li>撰寫軟體功能說明文件</li>
                                <li>撰寫研發文件</li>
                            </ul>
                        </div>
                    </div>
                    <div class="right">
                        <div class="box">
                            <div class="tt">需求年資與背景</div>
                            <ul>
                                <li>碩士畢業，2年以上經驗</li>
                                <li>電機電子工程、自動控制、資訊工程相關系所畢業</li>
                            </ul>
                        </div>
                        <div class="box">
                            <div class="tt">具備技能</div>
                            <ul>
                                <li>熟悉使用C、C#、C++</li>
                                <li>熟悉Open CASCADE或OpenCV尤佳</li>
                            </ul>
                        </div>
                    </div>
                </div><a class="btn js-monitor-params" href="https://www.104.com.tw/job/?jobno=5dmxf" target="_blank"><span>立即應徵</span><span class="icon"> <img src="../asset/svg/arrow.svg" alt=""></span></a>
                <div class="mt"><img src="../img/mt.png" alt=""></div>
                <div class="solar_box">
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                    <div class="solar"><img src="../asset/svg/solar.svg" alt=""></div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'wrapWorker',
        data () {
            return {
                loadHash: true,
                hash: '1'
            }
        },
        beforeMount: function(){
            var workerHash = (location.hash != '' && location.hash.indexOf('#hash') > -1) ? location.hash.replace('#hash', '') : '1';
            this.hash = workerHash;
        },
        methods: {
            hashSet: function(evt, num){
                if(evt) evt.preventDefault();
                this.hash = num;
                location.hash = '#hash' + num;
            }
        }
    }
</script>

<style>
    
</style>