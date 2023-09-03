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
                        도전하는 것은 항상 두려움을 동반합니다.
                        하지만 그와 동시에 새로운 즐거움을 추구할 수 있다고 생각합니다.
                        항상 도전하며, 부족하지만 성실히 노력하는
                        퍼블리셔가 되고 싶습니다.
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