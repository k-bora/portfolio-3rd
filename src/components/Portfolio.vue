
<template>
    <section id="port" class="section">
        <div class="container">
            <div class="sec">
                <div class="secHead">
                    <strong class="secHead__tit">Protfolio</strong>
                </div>
                <div class="portList">
                    <swiper
                        :slidesPerView="1"
                        :spaceBetween="30"
                        :loop="true"
                        :resistance="true"
                        :freeMode="true"
                        :pagination="{clickable: true,}"
                        :navigation="true"
                        :breakpoints="{
                            '769': {
                                slidesPerView: 1,
                                spaceBetween: 30,
                            },
                            '1080': {
                                slidesPerView: 3,
                                spaceBetween: 25,
                            },
                        }"
                        :modules="modules"
                        class="mySwiper">
                        <swiper-slide class="portList__item">
                            <div>
                                <strong class="tit">춘천시 디지털 신분증</strong>
                                <div class="imgBox"><img src="../assets/image/port_chuncheon.jpg"></div>
                                <div class="txtBox">
                                    <span class="txt">춘천시민을 위한 한번에 보는 디지털 신분증</span>
                                    <span class="txt">WEBAPP 플랫폼 제작, CMS 관리자</span>
                                </div>
                                <div class="workBox">
                                    <span class="work">UI/UX 퍼블리싱</span>
                                </div>
                            </div>
                            <div>
                            <!-- <a href="" target="_blank" class="btnLink">사이트 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a> -->
                            <a href="https://k-bora.github.io/portfolio-2nd/portfolio/014_chuncheon/app/html/app-main.html" target="_blank" class="btnLink">APP 메인 마크업 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                            <!-- <a href="https://k-bora.github.io/portfolio-2nd/portfolio/014_chuncheon/cms/html/app-main.html" target="_blank" class="btnLink">CMS 메인 마크업 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>     -->
                        </div>
                        </swiper-slide>
                        <swiper-slide class="portList__item">
                            <div>
                                <strong class="tit">블랙버드T</strong>
                                <div class="imgBox"><img src="../assets/image/port_blackbird.jpg"></div>
                                <div class="txtBox">
                                    <span class="txt">스마트 관광택시 예약 플랫폼 소개 홈페이지, WEBAPP</span>
                                    <span class="txt">PC/모바일 지원, 다국어 지원</span>
                                    <span class="txt">WEBAPP 플랫폼 제작, 고도화</span>
                                </div>
                                <div class="workBox">
                                    <span class="work">UI/UX 퍼블리싱</span>
                                </div>
                            </div>
                            <div>
                            <a href="https://www.blackbirdt.com/index.html" target="_blank" class="btnLink">사이트 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                            </div>
                        </swiper-slide>
                        <swiper-slide class="portList__item">
                            <div>
                                <strong class="tit">스마트 관광택시 청주여기</strong>
                                <div class="imgBox"><img src="../assets/image/port_cheongju.jpg"></div>
                                <div class="txtBox">
                                    <span class="txt">청주시에서 택시를 예약하여 코스여행 할수있는 모바일 웹앱</span>
                                    <span class="txt">안드로이드만 지원</span>
                                </div>
                                <div class="workBox">
                                    <span class="work">UI/UX 퍼블리싱</span>
                                </div>
                            </div>
                            <div>
                                <a href="https://k-bora.github.io/portfolio-2nd/portfolio/013_cheongju/webapp/pub/a.html" target="_blank" class="btnLink">추천코스 마크업 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                                <a href="https://k-bora.github.io/portfolio-2nd/portfolio/013_cheongju/webapp/pub/c.html" target="_blank" class="btnLink">채팅화면 마크업 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                            </div>
                        </swiper-slide>
                        <swiper-slide class="portList__item">
                            <div>
                                <strong class="tit">KT 이체인</strong>
                                <div class="imgBox"><img src="../assets/image/port_echain.jpg"></div>
                                <div class="txtBox">
                                    <span class="txt">KT에서 2050 탄소중립을 위한 KT의 플랫폼</span>
                                    <span class="txt">PC만 지원</span>
                                </div>
                                <div class="workBox">
                                    <span class="work">UI/UX 퍼블리싱</span>
                                </div>
                            </div>
                            <div>
                                <a href="https://k-bora.github.io/portfolio-2nd/portfolio/011_echain/pub/00_9_dashboard.html" target="_blank" class="btnLink">CMS 메인 마크업 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                                <a href="https://k-bora.github.io/portfolio-2nd/portfolio/011_echain/pub/00_0_mdLayout.html" target="_blank" class="btnLink">CMS 모듈 마크업 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                            </div>
                        </swiper-slide>
                        <swiper-slide class="portList__item">
                            <div>
                                <strong class="tit">KT 에너지 온실가스</strong>
                                <div class="imgBox"><img src="../assets/image/port_gas.jpg"></div>
                                <div class="txtBox">
                                    <span class="txt">KT의 온실가스 모니터링 CMS</span>
                                    <span class="txt">PC만 지원</span>
                                </div>
                                <div class="workBox">
                                    <span class="work">UI/UX 퍼블리싱</span>
                                </div>
                            </div>
                            <div>
                                <a href="https://k-bora.github.io/portfolio-2nd/portfolio/012_gas/html/01_1_dashboard_gas.html" target="_blank" class="btnLink">CMS 메인1 마크업 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                                <a href="https://k-bora.github.io/portfolio-2nd/portfolio/012_gas/html/01_3_dashboard_group.html" target="_blank" class="btnLink">CMS 메인2 마크업 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                            </div>
                        </swiper-slide>
                        <swiper-slide class="portList__item">
                            <div>
                                <strong class="tit">유어브랜드</strong>
                                <div class="imgBox"><img src="../assets/image/port_yourbrand.jpg"></div>
                                <div class="txtBox">
                                    <span class="txt">인플루언서의 브랜드를 만들고,그들의 코스메틱을 소개 및 판매하는 회사 홈페이지</span>
                                    <span class="txt">PC/모바일 지원</span>
                                </div>
                                <div class="workBox">
                                    <span class="work">web/cafe24 퍼블리싱</span>
                                    <span class="work">웹 디자인</span>
                                </div>
                            </div>
                            <div>
                                <a href="https://yourbrand.kr/" target="_blank" class="btnLink">사이트 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                            </div>
                        </swiper-slide>
                        <swiper-slide class="portList__item">
                            <div>
                                <strong class="tit">라벨리</strong>
                                <div class="imgBox"><img src="../assets/image/port_lavelee.jpg"></div>
                                <div class="txtBox">
                                    <span class="txt">라벨리 회사소개 홈페이지</span>
                                    <span class="txt">PC/모바일 지원</span>
                                </div>
                                <div class="workBox">
                                    <span class="work">web/wordpress 퍼블리싱</span>
                                    <span class="work">웹 디자인</span>
                                </div>
                            </div>
                            <div>
                                <a href="https://lavelee.co.kr/" target="_blank" class="btnLink">사이트 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                            </div>
                        </swiper-slide>
                        <swiper-slide class="portList__item">
                            <div>
                                <strong class="tit">스토랑트</strong>
                                <div class="imgBox"><img src="../assets/image/port_storant.jpg"></div>
                                <div class="txtBox">
                                    <span class="txt">스토랑트 무인 카페 브랜드 소개 홈페이지</span>
                                    <span class="txt">PC/모바일 지원</span>
                                </div>
                                <div class="workBox">
                                    <span class="work">web/mir9 퍼블리싱</span>
                                    <span class="work">웹 디자인</span>
                                </div>
                            </div>
                            <div>
                                <a href="http://www.storant.co.kr/main" target="_blank" class="btnLink">사이트 보러가기 <svg class="arrowRight" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 34.2 32.3" xml:xpace="preserve" style="stroke-width: 2;"><line x1="0" y1="16" x2="33" y2="16"></line><line x1="17.3" y1="0.7" x2="33.2" y2="16.5"></line><line x1="17.3" y1="31.6" x2="33.5" y2="15.4"></line></svg></a>
                            </div>
                        </swiper-slide>
                    </swiper>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
  import { Swiper, SwiperSlide } from 'swiper/vue';
  import 'swiper/css';
  import 'swiper/css/pagination';
  import 'swiper/css/navigation';
  import { Pagination, Navigation } from 'swiper/modules';

export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
         modules: [Pagination, Navigation]
      };
    },
};
</script>





