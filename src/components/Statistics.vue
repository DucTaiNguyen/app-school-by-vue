
<template>
  <div class="home-container">
    <div class="home-container1">
      <div class="home-master-header">
        <h1 class="home-text">
          <span class="home-text01">THE AMERICAN UNIVERSITY <small>OF</small>  PARIS</span>
        </h1>
      </div>
      <div class="home-container2">
        <h1 class="home-text02">
          <span class="home-text03">A</span>
          <span>pply </span>
          <span class="home-text05">S</span>
          <span class="home-text06"></span>
          <span>tatistics </span>
          <span class="home-text08">I</span>
          <!-- <span class="home-text09"></span> -->
          <!-- <span></span> -->
        </h1>
        <h2 class="home-text11">Data Sciences</h2>
      </div>
      <div class="home-menu">
        <div class="home-right-item">
          <a
            href="https://example.com"
            target="_blank"
            rel="noreferrer noopener"
            class="thqLink"
          >
            Home
          </a>
          <a
            href="https://example.com"
            target="_blank"
            rel="noreferrer noopener"
            class="thqLink"
          >
            Courses
          </a>
          <a
            href="https://example.com"
            target="_blank"
            rel="noreferrer noopener"
            class="thqLink"
          >
            Using SE
          </a>
        </div>
        <div class="home-left-item">
          <a
            href="https://example.com"
            target="_blank"
            rel="noreferrer noopener"
            class="thqLink home-link3"
          >
            SURVEY
          </a>
          <a
            href="https://example.com"
            target="_blank"
            rel="noreferrer noopener"
            class="thqLink home-link4"
          >
            CONTACT US
          </a>
        </div>
      </div>
      <div class="home-content">
        <div class="home-course-details">
          <div class="home-accodiance">
            <span><span class="home-text13">Course Details</span></span>
            <span class="home-text14">Show All</span>
          </div>

          <Accordion
            v-for="(course, index) in courses"
            :key="index"
            :title="course.title"
            :description="course.description"
          />
        </div>
        <div class="home-course-sessions">
          <div class="home-accodiance06">
            <span class="home-text25">Course Details</span>
            <span class="home-text26"
              ><span class="home-text27">Show All</span></span
            >
          </div>
          <Lecture
            v-for="(lecture, index) in lectures"
            :key="index"
            :lecture="index + 1"
            :mylink="lecture.mylink"
            :lectureTitle="lecture.lectureTitle"
          />
        </div>
      </div>
    </div>

    <div class="home-footer">
      <div class="home-footer-top">
        <div class="home-footer-top-right">
          <span class="home-text68">AUP |</span>
          <span class="home-text69">
            <span>
              Center
              <span v-html="rawedj0"></span>
            </span>
            <span>for</span>
            <br />
            <span>profestional develpment</span>
          </span>
        </div>
        <span>Contact Us</span>
        <div class="home-footer-top-left">
          <svg viewBox="0 0 877.7142857142857 1024" class="home-icon">
            <path
              d="M713.143 73.143c90.857 0 164.571 73.714 164.571 164.571v548.571c0 90.857-73.714 164.571-164.571 164.571h-107.429v-340h113.714l17.143-132.571h-130.857v-84.571c0-38.286 10.286-64 65.714-64l69.714-0.571v-118.286c-12-1.714-53.714-5.143-101.714-5.143-101.143 0-170.857 61.714-170.857 174.857v97.714h-114.286v132.571h114.286v340h-304c-90.857 0-164.571-73.714-164.571-164.571v-548.571c0-90.857 73.714-164.571 164.571-164.571h548.571z"
            ></path></svg
          ><svg viewBox="0 0 877.7142857142857 1024" class="home-icon02">
            <path
              d="M585.143 512c0-80.571-65.714-146.286-146.286-146.286s-146.286 65.714-146.286 146.286 65.714 146.286 146.286 146.286 146.286-65.714 146.286-146.286zM664 512c0 124.571-100.571 225.143-225.143 225.143s-225.143-100.571-225.143-225.143 100.571-225.143 225.143-225.143 225.143 100.571 225.143 225.143zM725.714 277.714c0 29.143-23.429 52.571-52.571 52.571s-52.571-23.429-52.571-52.571 23.429-52.571 52.571-52.571 52.571 23.429 52.571 52.571zM438.857 152c-64 0-201.143-5.143-258.857 17.714-20 8-34.857 17.714-50.286 33.143s-25.143 30.286-33.143 50.286c-22.857 57.714-17.714 194.857-17.714 258.857s-5.143 201.143 17.714 258.857c8 20 17.714 34.857 33.143 50.286s30.286 25.143 50.286 33.143c57.714 22.857 194.857 17.714 258.857 17.714s201.143 5.143 258.857-17.714c20-8 34.857-17.714 50.286-33.143s25.143-30.286 33.143-50.286c22.857-57.714 17.714-194.857 17.714-258.857s5.143-201.143-17.714-258.857c-8-20-17.714-34.857-33.143-50.286s-30.286-25.143-50.286-33.143c-57.714-22.857-194.857-17.714-258.857-17.714zM877.714 512c0 60.571 0.571 120.571-2.857 181.143-3.429 70.286-19.429 132.571-70.857 184s-113.714 67.429-184 70.857c-60.571 3.429-120.571 2.857-181.143 2.857s-120.571 0.571-181.143-2.857c-70.286-3.429-132.571-19.429-184-70.857s-67.429-113.714-70.857-184c-3.429-60.571-2.857-120.571-2.857-181.143s-0.571-120.571 2.857-181.143c3.429-70.286 19.429-132.571 70.857-184s113.714-67.429 184-70.857c60.571-3.429 120.571-2.857 181.143-2.857s120.571-0.571 181.143 2.857c70.286 3.429 132.571 19.429 184 70.857s67.429 113.714 70.857 184c3.429 60.571 2.857 120.571 2.857 181.143z"
            ></path></svg
          ><svg viewBox="0 0 877.7142857142857 1024" class="home-icon04">
            <path
              d="M525.143 744.571v-89.714c0-18.857-5.714-28.571-16.571-28.571-6.286 0-12.571 2.857-18.857 9.143v128c6.286 6.286 12.571 9.143 18.857 9.143 10.857 0 16.571-9.143 16.571-28zM630.286 674.857h37.714v-19.429c0-19.429-6.286-29.143-18.857-29.143s-18.857 9.714-18.857 29.143v19.429zM304 522.857v40h-45.714v241.714h-42.286v-241.714h-44.571v-40h132.571zM418.857 594.857v209.714h-38.286v-22.857c-14.857 17.143-29.143 25.714-43.429 25.714-12 0-20.571-5.143-24-16-2.286-6.286-3.429-16-3.429-30.857v-165.714h37.714v154.286c0 8.571 0 13.714 0.571 14.857 0.571 5.714 3.429 8.571 8.571 8.571 8 0 15.429-5.714 24-17.714v-160h38.286zM562.857 658.286v83.429c0 18.857-1.143 33.143-4 41.714-4.571 16-14.857 24-30.286 24-13.143 0-26.286-8-38.857-23.429v20.571h-38.286v-281.714h38.286v92c12-14.857 25.143-22.857 38.857-22.857 15.429 0 25.714 8 30.286 24 2.857 8.571 4 22.286 4 42.286zM706.286 732v5.143c0 12.571-0.571 20.571-1.143 24.571-1.143 8.571-4 16-8.571 22.857-10.286 15.429-26.286 22.857-45.714 22.857-20 0-35.429-7.429-46.286-21.714-8-10.286-12-26.857-12-49.143v-73.714c0-22.286 3.429-38.286 11.429-49.143 10.857-14.286 26.286-21.714 45.714-21.714 18.857 0 34.286 7.429 44.571 21.714 8 10.857 12 26.857 12 49.143v43.429h-76v37.143c0 19.429 6.286 29.143 19.429 29.143 9.143 0 14.857-5.143 17.143-14.857 0-2.286 0.571-10.857 0.571-25.714h38.857zM448.571 261.143v89.143c0 19.429-6.286 29.143-18.286 29.143-12.571 0-18.286-9.714-18.286-29.143v-89.143c0-19.429 5.714-29.714 18.286-29.714 12 0 18.286 10.286 18.286 29.714zM753.143 668.571v0c0-49.143 0-101.143-10.857-148.571-8-33.714-35.429-58.286-68-61.714-77.714-8.571-156.571-8.571-235.429-8.571-78.286 0-157.143 0-234.857 8.571-33.143 3.429-60.571 28-68 61.714-10.857 47.429-11.429 99.429-11.429 148.571v0c0 48.571 0 100.571 11.429 148.571 7.429 33.143 34.857 57.714 67.429 61.714 78.286 8.571 157.143 8.571 235.429 8.571s157.143 0 235.429-8.571c32.571-4 60-28.571 67.429-61.714 11.429-48 11.429-100 11.429-148.571zM321.714 296.571l51.429-169.143h-42.857l-29.143 111.429-30.286-111.429h-44.571c8.571 26.286 18.286 52.571 26.857 78.857 13.714 40 22.286 69.714 26.286 90.286v114.857h42.286v-114.857zM486.857 342.857v-74.286c0-22.286-4-38.857-12-49.714-10.857-14.286-25.714-21.714-44.571-21.714-19.429 0-34.286 7.429-44.571 21.714-8 10.857-12 27.429-12 49.714v74.286c0 22.286 4 38.857 12 49.714 10.286 14.286 25.143 21.714 44.571 21.714 18.857 0 33.714-7.429 44.571-21.714 8-10.286 12-27.429 12-49.714zM590.286 411.429h38.286v-211.429h-38.286v161.714c-8.571 12-16.571 17.714-24 17.714-5.143 0-8.571-2.857-9.143-9.143-0.571-1.143-0.571-5.714-0.571-14.857v-155.429h-38.286v167.429c0 14.857 1.143 24.571 3.429 31.429 4 10.286 12.571 15.429 24.571 15.429 14.286 0 28.571-8.571 44-25.714v22.857zM877.714 237.714v548.571c0 90.857-73.714 164.571-164.571 164.571h-548.571c-90.857 0-164.571-73.714-164.571-164.571v-548.571c0-90.857 73.714-164.571 164.571-164.571h548.571c90.857 0 164.571 73.714 164.571 164.571z"
            ></path></svg
          ><svg viewBox="0 0 1316.5714285714284 1024" class="home-icon06">
            <path
              d="M821.143 521.714c0 239.429-160.571 409.143-402.286 409.143-231.429 0-418.857-187.429-418.857-418.857s187.429-418.857 418.857-418.857c113.143 0 207.429 41.143 280.571 109.714l-113.714 109.143c-30.857-29.714-85.143-64.571-166.857-64.571-142.857 0-259.429 118.286-259.429 264.571s116.571 264.571 259.429 264.571c165.714 0 228-119.429 237.714-180.571h-237.714v-144h395.429c4 21.143 6.857 42.286 6.857 69.714zM1316.571 452v120h-119.429v119.429h-120v-119.429h-119.429v-120h119.429v-119.429h120v119.429h119.429z"
            ></path></svg
          ><svg viewBox="0 0 877.7142857142857 1024" class="home-icon08">
            <path
              d="M135.429 808h132v-396.571h-132v396.571zM276 289.143c-0.571-38.857-28.571-68.571-73.714-68.571s-74.857 29.714-74.857 68.571c0 37.714 28.571 68.571 73.143 68.571h0.571c46.286 0 74.857-30.857 74.857-68.571zM610.286 808h132v-227.429c0-121.714-65.143-178.286-152-178.286-70.857 0-102.286 39.429-119.429 66.857h1.143v-57.714h-132s1.714 37.143 0 396.571v0h132v-221.714c0-11.429 0.571-23.429 4-32 9.714-23.429 31.429-48 68-48 47.429 0 66.286 36 66.286 89.714v212zM877.714 237.714v548.571c0 90.857-73.714 164.571-164.571 164.571h-548.571c-90.857 0-164.571-73.714-164.571-164.571v-548.571c0-90.857 73.714-164.571 164.571-164.571h548.571c90.857 0 164.571 73.714 164.571 164.571z"
            ></path>
          </svg>
        </div>
      </div>
      <div class="home-footer-bottom">
        <div class="home-footer-bottom-left">
          <span class="home-text75"><span>AUP</span></span>
          <span class="home-text77">University</span>
        </div>
        <div class="home-footer-bottom-right">
          <div class="home-footer-content">
            <span class="home-text78">AUP Home</span>
            <span class="home-text79">Maps &amp; Directions</span>
            <span class="home-text80">Search AUP</span>
            <span class="home-text81">Emergency Info</span>
          </div>
          <div class="home-footer-content1">
            <span class="home-text82">Terms of Use</span>
            <span class="home-text83">Privacy</span>
            <span class="home-text84">Copyright</span>
            <span class="home-text85">Trademarks</span>
            <span class="home-text86">Non-Discrimination</span>
            <span class="home-text87">Accessibility</span>
          </div>
          <div class="home-footer-content2">
            <span class="home-text88">© AUP University</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Accordion from "./Accordion";
import Lecture from "./Lecture";
export default {
  name: "Home",
  components: {
    Accordion,
    Lecture,
  },
  data() {
    return {
    
/////////////////////////////////////////

 
courses: [
{
    title: "Course Description",
    description: `The course Applied Statistics introduces the basic tools of descriptive and inferential statistical analysis. In this course, we will cover the data-analysis concepts and procedures used in economics,
business and other social sciences. Emphasis will be given to the manipulation of real data sets to obtain useful and meaningful statistical results, to the qualitative interpretation of such results and to the effective communication in numbers, graphs and words of the insights thus developed. Theory will be combined with data collection and curation, as well as computer lab work with a statistical software package. Students will be encouraged to develop an attitude of mind that accepts uncertainty and variability as part of problem analysis and decision making.
The only prerequisite for this course is your mathematics courses at high school. The content of this course is covered by the textbook, we will discuss it according to the tentative schedule. There will be homework, quizzes, labs, midterm and final exams.`,
},
{
    title: "Instructor",
    description: `Quang Nguyen-Luong`,
},
],


lectures: [
{
    lectureTitle:"Introduction to Statistics",
    duration:"",
    mylink:{
    watchNow:"https://www.youtube.com/watch?v=KBLQ7GJLlQE",
    download:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    html:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    pdf:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    datadesk:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    excel:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    R:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    python:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
} 
},

{
lectureTitle:" Categorical data",
duration:"",
mylink:{
    watchNow:"https://www.youtube.com/watch?v=KBLQ7GJLlQE",
    download:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    html:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    pdf:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    datadesk:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    excel:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    R:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    python:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
} 
},

{
lectureTitle:" Quantitative data ",
duration:"",
mylink:{
    watchNow:"https://www.youtube.com/watch?v=KBLQ7GJLlQE",
    download:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    html:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    pdf:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    datadesk:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    excel:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    R:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
    python:" https://drive.google.com/file/d/12L0GFAsiOHtSs3nj58anVQrMXHi8izmx/view?usp=sharing ",
} 
},

],




      ////////////////////////// 
        
     
    };
  },
};
</script>

<style >
.home-container {
  width: 100%;
  height: auto;
  display: flex;
  min-height: 100vh;
  align-items: center;
  flex-direction: column;
  justify-content: flex-start;
}
.home-container1 {
  flex: 0 0 auto;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: flex-start;
  padding-top: var(--dl-space-space-doubleunit);

  flex-direction: column;
  padding-bottom: var(--dl-space-space-doubleunit);
}
.home-master-header {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
  background-color:  var(--main-cl);
}
.home-text {
  font-size: 25px;
  align-self: flex-start;
}
.home-text01 {
  color: var(--dl-color-gray-white);
}
.home-container2 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
}
.home-text02 {
  align-self: center;
}
.home-text03 {
  color:  var(--main-cl);
  text-transform: uppercase;
}
.home-text05 {
  color:  var(--main-cl);
}
.home-text06 {
  color:  var(--main-cl);
}
.home-text08 {
  color:  var(--main-cl);
}
.home-text09 {
  color:  var(--main-cl);
}
.home-text11 {
  align-self: center;
  margin-left: auto;
}
.home-menu {
  flex: 0 0 auto;
  width: 100%;
  height: var(--dl-size-size-doubleunit);
  display: flex;
  margin-top: 10px;
  align-items: flex-start;
  flex-direction: row;
}
.home-right-item {
  width: 264px;
  display: flex;
  align-self: center;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
}
.home-left-item {
  width: 187px;
  display: flex;
  align-self: center;
  align-items: flex-start;
  margin-left: auto;
  flex-direction: row;
  justify-content: space-between;
}
.home-link3 {
  font-size: 14px;
  align-self: center;
}
.home-link4 {
  font-size: 14px;
  align-self: center;
}
.home-content {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.home-course-details {
  flex: 0 0 auto;
  width: 48%;
  display: flex;
  position: relative;
  align-self: flex-start;
  align-items: flex-start;
  grid-row-gap: 3px;
  margin-right: 0px;
  padding-right: 0px;
  flex-direction: column;
}
.home-accodiance {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  background-color: #555246;
}
.home-text13 {
  color: var(--dl-color-gray-white);
}
.home-text14 {
  color: var(--dl-color-gray-white);

  margin-right: var(--dl-space-space-unit);
}
.home-accodiance01 {
  top: 28px;
  flex: 0 0 auto;
  left: auto;
  right: 0px;
  width: 100%;
  bottom: auto;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text16 {
  padding-right: var(--dl-space-space-unit);
}
.home-accodiance02 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text18 {
  transition: 0.3s;
  padding-right: var(--dl-space-space-unit);
}
.home-accodiance03 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text20 {
  transition: 0.3s;
  padding-right: var(--dl-space-space-unit);
}
.home-accodiance04 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text22 {
  transition: 0.3s;
  padding-right: var(--dl-space-space-unit);
}
.home-accodiance05 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text24 {
  transition: 0.3s;
  padding-right: var(--dl-space-space-unit);
}
.home-course-sessions {
  flex: 0 0 auto;
  width: 48%;
  display: flex;
  align-items: flex-start;
  grid-row-gap: 3px;
  margin-right: 0px;
  padding-right: 0px;
  flex-direction: column;
}
.home-accodiance06 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  background-color: #555246;
}
.home-text25 {
  color: var(--dl-color-gray-white);
}
.home-text26 {
  margin-right: var(--dl-space-space-unit);
}
.home-text27 {
  color: var(--dl-color-gray-white);
}
.home-accodiance07 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text29 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance08 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text31 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance09 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text33 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance10 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text35 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance11 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text37 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance12 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text39 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance13 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text41 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance14 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text43 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance15 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text45 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance16 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text47 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance17 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text49 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance18 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text51 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance19 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text53 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance20 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text55 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance21 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text57 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance22 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text59 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance23 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text61 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance24 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text63 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance25 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text65 {
  margin-right: var(--dl-space-space-unit);
}
.home-accodiance26 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  margin-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.home-text67 {
  margin-right: var(--dl-space-space-unit);
}
.home-footer {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.home-footer-top {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.home-footer-top-right {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: flex-start;
}
.home-text68 {
  font-size: 30px;
}
.home-text69 {
  font-size: 20px;
  line-height: 1;
  margin-left: var(--dl-space-space-halfunit);
}
.home-footer-top-left {
  width: 240px;
  height: 100px;
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.home-icon {
  width: 36px;
  height: 36px;
}
.home-icon02 {
  width: 36px;
  height: 36px;
}
.home-icon04 {
  width: 36px;
  height: 36px;
}
.home-icon06 {
  width: 36px;
  height: 36px;
}
.home-icon08 {
  width: 36px;
  height: 36px;
}
.home-footer-bottom {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  padding-top: var(--dl-space-space-doubleunit);
  flex-direction: row;
  justify-content: flex-start;
  background-color:  var(--main-cl);
}
.home-footer-bottom-left {
  flex: 0 0 auto;
  width: 200px;
  height: 100px;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.home-text75 {
  color: var(--dl-color-gray-white);
  font-size: 30px;
  line-height: 1;
}
.home-text77 {
  color: var(--dl-color-gray-white);
  font-size: 25px;
  line-height: 1;
  padding-top: 0px;
}
.home-footer-bottom-right {
  flex: 0 0 auto;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}
.home-footer-content {
  display: flex;
  align-items: center;
  flex-direction: row;
  padding-bottom: var(--dl-space-space-halfunit);
  justify-content: space-between;
}
.home-text78 {
  color: var(--dl-color-gray-white);
  padding-right: var(--dl-space-space-unit);
}
.home-text79 {
  color: var(--dl-color-gray-white);
  padding-right: var(--dl-space-space-unit);
}
.home-text80 {
  color: var(--dl-color-gray-white);
  padding-right: var(--dl-space-space-unit);
}
.home-text81 {
  color: var(--dl-color-gray-white);
}
.home-footer-content1 {
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: row;
  padding-bottom: var(--dl-space-space-halfunit);
  justify-content: space-between;
}
.home-text82 {
  color: var(--dl-color-gray-white);

  padding-right: var(--dl-space-space-unit);
}
.home-text83 {
  color: var(--dl-color-gray-white);

  padding-right: var(--dl-space-space-unit);
}
.home-text84 {
  color: var(--dl-color-gray-white);

  padding-right: var(--dl-space-space-unit);
}
.home-text85 {
  color: var(--dl-color-gray-white);

  padding-right: var(--dl-space-space-unit);
}
.home-text86 {
  color: var(--dl-color-gray-white);

  padding-right: var(--dl-space-space-unit);
}
.home-text87 {
  color: var(--dl-color-gray-white);
}
.home-footer-content2 {
  display: flex;
  align-items: center;
  flex-direction: row;
  padding-bottom: var(--dl-space-space-halfunit);
  justify-content: space-between;
}
.home-text88 {
  color: var(--dl-color-gray-white);
}
.badger-accordion__header {
  width: 100%;
}

.js-badger-accordion.home-course-details.badger-accordion--initialized {
  width: 100%;
}
.badger-accordion__header .js-badger-accordion-header .badger-accordion-toggle {
  background: rgb(46, 202, 200) !important;
}

@media (max-width: 768px) {
  .home-text {
    font-size: 1.2rem;
  }
  .home-content {
    flex-direction: column;
  }
  .home-course-details {
    width: 100%;
  }
  .home-course-sessions {
    width: 100%;
  }
  .home-text58 {
    font-size: 25px;
  }
  .home-text59 {
    font-size: 18px;
  }
  .home-footer-bottom {
    flex-direction: column;
  }
  .home-footer-bottom-left {
    width: auto;
    height: auto;
    flex-direction: column;
  }
  .home-footer-bottom-right {
    align-items: center;
    flex-direction: column;
  }
  .home-footer-content {
    flex-direction: row;
  }
  .home-footer-content1 {
    width: auto;
    flex-direction: row;
  }
}
@media (max-width: 576px) {
  .home-container2 {
    flex-direction: column;
  }
  .home-text02 {
    font-size: 1.5rem;
  }
  .home-text11 {
    font-size: 1.5rem;
    align-self: center;
    margin-left: 0px;
  }
  .home-content {
    width: 100%;
    height: auto;
    align-items: center;
    flex-direction: column;
  }
  .home-course-details {
    width: 100%;
  }
  .home-course-sessions {
    width: 100%;
  }
  .home-footer-top {
    flex-direction: column;
  }
  .home-footer-top-right {
    flex-direction: row;
  }
  .home-text58 {
    font-size: 20px;
  }
  .home-text59 {
    font-size: 18px;
  }
  .home-footer-top-left {
    width: auto;
    height: auto;
  }
}
@media (max-width: 425px) {
  .home-menu {
    height: auto;
    align-items: center;
    margin-bottom: var(--dl-space-space-halfunit);
    justify-content: space-between;
  }
  .home-link {
    font-size: 14px;
  }
  .home-link1 {
    font-size: 14px;
  }
  .home-link2 {
    font-size: 14px;
  }
  .home-left-item {
    align-items: center;
    margin-left: var(--dl-space-space-halfunit);
    justify-content: space-between;
  }
  .home-link3 {
    font-size: 14px;
    align-self: center;
    padding-left: var(--dl-space-space-halfunit);
    padding-right: 0px;
    text-transform: lowercase;
  }
  .home-link4 {
    text-transform: lowercase;
  }
  .home-content {
    width: 100%;
    height: auto;
    align-items: center;
    flex-direction: column;
  }
  .home-course-details {
    width: 100%;
  }
  .home-course-sessions {
    width: 100%;
  }
  .home-footer-top {
    padding-top: var(--dl-space-space-halfunit);
    flex-direction: column;
    padding-bottom: var(--dl-space-space-halfunit);
  }
  .home-footer-top-right {
    flex-direction: row;
  }
  .home-text58 {
    font-size: 20px;
  }
  .home-text59 {
    font-size: 18px;
  }
  .home-footer-top-left {
    width: auto;
    height: auto;
  }
  .home-icon {
    width: 24px;
    height: 24px;
  }
  .home-icon02 {
    width: 24px;
    height: 24px;
  }
  .home-icon04 {
    width: 24px;
    height: 24px;
  }
  .home-icon06 {
    width: 24px;
    height: 24px;
  }
  .home-icon08 {
    width: 24px;
    height: 24px;
  }
  .home-footer-content {
    flex-direction: column;
  }
  .home-footer-content1 {
    flex-direction: column;
  }
  .home-text79 {
    text-align: center;
  }
}
@media (max-width: 576px) {
  .home-menu {
    height: auto;
    align-items: center;
    margin-bottom: var(--dl-space-space-halfunit);
    justify-content: space-between;
  }
  .home-link {
    font-size: 14px;
  }
  .home-link1 {
    font-size: 14px;
  }
  .home-link2 {
    font-size: 14px;
  }
  .home-left-item {
    align-items: center;
    margin-left: var(--dl-space-space-halfunit);
    justify-content: space-between;
  }
  .home-link3 {
    font-size: 14px;
    align-self: center;
    padding-left: var(--dl-space-space-halfunit);
    padding-right: 0px;
    text-transform: lowercase;
  }
  .home-link4 {
    text-transform: lowercase;
  }
  .home-content {
    width: 100%;
    height: auto;
    align-items: center;
    flex-direction: column;
  }
  .home-course-details {
    width: 100%;
  }
  .home-course-sessions {
    width: 100%;
  }
  .home-footer-top {
    padding-top: var(--dl-space-space-halfunit);
    flex-direction: column;
    padding-bottom: var(--dl-space-space-halfunit);
  }
  .home-footer-top-right {
    flex-direction: row;
  }
  .home-text58 {
    font-size: 20px;
  }
  .home-text59 {
    font-size: 18px;
  }
  .home-footer-top-left {
    width: auto;
    height: auto;
  }
  .home-icon {
    width: 24px;
    height: 24px;
  }
  .home-icon02 {
    width: 24px;
    height: 24px;
  }
  .home-icon04 {
    width: 24px;
    height: 24px;
  }
  .home-icon06 {
    width: 24px;
    height: 24px;
  }
  .home-icon08 {
    width: 24px;
    height: 24px;
  }
  .home-footer-content {
    flex-direction: column;
  }
  .home-footer-content1 {
    flex-direction: column;
  }
  .home-text79 {
    text-align: center;
  }
}
</style>
