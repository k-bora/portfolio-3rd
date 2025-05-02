<script setup>
import { workList , eduList , licenseList , skillList } from "@/constants/list";

</script>
<template>
    <section id="home" class="section">
        <div class="container">
            <div class="about">
                <div class="profile">
                    <div class="sticky">
                        <div class="perspective">
                            <div class="profile__cont">
                                <img class="profile__img" src="../assets/image/profile.png" alt="인사하는 미모티콘">
                                <strong class="profile__name">KIM BORA</strong>
                                <ul class="socialList">
                                    <li class="socialList__item">
                                        <a class="socialList__link socialList__link--tistory" target="_blank" href="https://pub-kim.tistory.com/" title="Tistory"><span class="blind">Tistory</span></a>
                                    </li>
                                    <li class="socialList__item">
                                        <a class="socialList__link socialList__link--github" target="_blank" href="https://github.com/k-bora/portfolio-3rd" title="Github"><span class="blind">Github</span></a>
                                    </li>
                                    <li class="socialList__item">
                                        <a class="socialList__link socialList__link--notion" target="_blank" href="https://elegant-colt-81d.notion.site/92f006eac2594dd0afa4a42efb05d32b?pvs=4" title="기술경력서"><span class="blind">기술경력서</span></a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="introduce">
                    <p class="introduce__text">
                        <strong class="hello">안녕하세요 :&#41;</strong>
                        사용자에게 더 나은 경험을 전달하는 퍼블리싱과 프론트엔드 개발에 관심이 많습니다.
                        두려움보다는 설렘으로, 부족함보다는 성실함으로 한 걸음씩 나아가고 있습니다.
                        작은 변화에 책임을 다하며, 팀에 꼭 필요한 사람이 되고 싶습니다.
                    </p>
                    <div class="sec" id="about">
                        <div class="secHead">
                            <strong class="secHead__tit">Work Experience</strong>
                        </div>
                        <ul class="introList">
                            <li class="introList__item" v-for="(work, key) in workList" :key="key">
                                <span class="introList__date">
                                    <span class="startDate">{{ work.startDate }}</span> - <span class="endDate">{{ work.endDate }}</span>
                                </span>
                                <div class="introInfo">
                                    <strong class="introInfo__name">{{ work.title }}</strong>
                                    <span class="introInfo__txt">{{ work.text }}</span>
                                </div>
                            </li>
                        </ul>
                    </div>
                    <div class="sec">
                        <div class="secHead">
                            <strong class="secHead__tit">Education</strong>
                        </div>
                        <ul class="introList">
                            <li class="introList__item" v-for="(edu, key) in eduList" :key="key">
                                <span class="introList__date">
                                    <span class="startDate">{{ edu.startDate }}</span> - <span class="endDate">{{ edu.endDate }}</span>
                                </span>
                                <div class="introInfo">
                                    <strong class="introInfo__name">{{ edu.title }}</strong>
                                    <span class="introInfo__txt">{{ edu.text }}</span>
                                </div>
                            </li>
                        </ul>
                    </div>
                    <div class="sec">
                        <div class="secHead secHead--skills">
                            <strong class="secHead__tit">Skills</strong>
                        </div>
                        <ul class="tags">
                            <li class="tags__item" v-for="(skill, key) in skillList" :key="key">{{ skill.name }}</li>
                        </ul>
                    </div>
                    <div class="sec" style="display: none;"> <!-- 정처기 취득후 등록 예정 -->
                        <div class="secHead">
                            <strong class="secHead__tit">License</strong>
                        </div>
                        <ul class="introList">
                            <li class="introList__item" v-for="(license, key) in licenseList" :key="key">
                                <span class="introList__date">
                                    <span class="endDate">{{ license.date }}</span>
                                </span>
                                <div class="introInfo">
                                    <span>{{ license.name }}</span>
                                    <span>{{ license.institution }}</span>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>