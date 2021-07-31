<template>
  <div class="lecture-detail-container">
    <div class="lecture-detail-container01">
      <div class="lecture-detail-container02">
        <div class="lecture-detail-title" @click="open = !open">
          <span class="lecture-detail-text">
            Class {{ lecture }} {{ lectureTitle }}</span
          >
          <span class="lecture-detail-text01">{{ sign }}</span>
        </div>
      </div>
      <div class="lecture-detail-container03" v-show="open">
        <div class="lecture-detail-container04">
          <a
            :href="mylink.watchNow"
            target="_blank"
            rel="noreferrer noopener"
            class="lecture-detail-link"
          >
            <div class="thqLink lecture-detail-watch-now">
              <svg
                viewBox="0 0 877.7142857142857 1024"
                class="lecture-detail-icon"
              >
                <path
                  d="M676.571 512c0 13.143-6.857 25.143-18.286 31.429l-310.857 182.857c-5.714 3.429-12 5.143-18.286 5.143s-12.571-1.714-18.286-4.571c-11.429-6.857-18.286-18.857-18.286-32v-365.714c0-13.143 6.857-25.143 18.286-32 11.429-6.286 25.714-6.286 36.571 0.571l310.857 182.857c11.429 6.286 18.286 18.286 18.286 31.429zM749.714 512c0-171.429-139.429-310.857-310.857-310.857s-310.857 139.429-310.857 310.857 139.429 310.857 310.857 310.857 310.857-139.429 310.857-310.857zM877.714 512c0 242.286-196.571 438.857-438.857 438.857s-438.857-196.571-438.857-438.857 196.571-438.857 438.857-438.857 438.857 196.571 438.857 438.857z"
                ></path>
              </svg>
              <span class="lecture-detail-text06">{{ text4 }}</span>
            </div>
          </a>
          <div class="lecture-detail-container05">
            <span>{{ text1 }}</span>
          </div>
          <span class="lecture-detail-text05">{{ text2 }}</span>
        </div>
        <div class="lecture-detail-container06">
          <span class="lecture-detail-text02">{{ duration }}</span>
          <a
            :href="mylink.download"
            target="_blank"
            rel="noreferrer noopener"
            class="lecture-detail-link1"
          >
            <div class="thqLink lecture-detail-download">
              <svg
                viewBox="0 0 950.8571428571428 1024"
                class="lecture-detail-icon2"
              >
                <path
                  d="M731.429 768c0-20-16.571-36.571-36.571-36.571s-36.571 16.571-36.571 36.571 16.571 36.571 36.571 36.571 36.571-16.571 36.571-36.571zM877.714 768c0-20-16.571-36.571-36.571-36.571s-36.571 16.571-36.571 36.571 16.571 36.571 36.571 36.571 36.571-16.571 36.571-36.571zM950.857 640v182.857c0 30.286-24.571 54.857-54.857 54.857h-841.143c-30.286 0-54.857-24.571-54.857-54.857v-182.857c0-30.286 24.571-54.857 54.857-54.857h265.714l77.143 77.714c21.143 20.571 48.571 32 77.714 32s56.571-11.429 77.714-32l77.714-77.714h265.143c30.286 0 54.857 24.571 54.857 54.857zM765.143 314.857c5.714 13.714 2.857 29.714-8 40l-256 256c-6.857 7.429-16.571 10.857-25.714 10.857s-18.857-3.429-25.714-10.857l-256-256c-10.857-10.286-13.714-26.286-8-40 5.714-13.143 18.857-22.286 33.714-22.286h146.286v-256c0-20 16.571-36.571 36.571-36.571h146.286c20 0 36.571 16.571 36.571 36.571v256h146.286c14.857 0 28 9.143 33.714 22.286z"
                ></path>
              </svg>
            </div>
          </a>
          <div class="lecture-detail-duration">
            <a
              :href="mylink.html"
              target="_blank"
              rel="noreferrer noopener"
              class="lecture-detail-link1"
            >
              <button class="thqButton lecture-detail-button">
                {{ button4 }}
              </button>
            </a>

            <a
              :href="mylink.pdf"
              target="_blank"
              rel="noreferrer noopener"
              class="lecture-detail-link1"
            >
              <button class="thqButton lecture-detail-button">
                {{ button5 }}
              </button>
            </a>
          </div>
        </div>

        <div class="lecture-detail-container08">
          <span class="lecture-detail-text10">{{ text6 }}</span>
          <span class="lecture-detail-text10">{{ text7 }}</span>
        </div>
        <div class="lecture-detail-container09">
          <div class="practice-btn">
            <a
              :href="mylink.datadesk"
              target="_blank"
              rel="noreferrer noopener"
              class="lecture-detail-link1"
            >
              <button class="thqButton lecture-detail-button">
                {{ button }}
              </button>
            </a>

            <a
              :href="mylink.excel"
              target="_blank"
              rel="noreferrer noopener"
              class="lecture-detail-link1"
            >
              <button class="thqButton lecture-detail-button">
                {{ button1 }}
              </button>
            </a>

            <a
              :href="mylink.R"
              target="_blank"
              rel="noreferrer noopener"
              class="lecture-detail-link1"
            >
              <button class="thqButton lecture-detail-button">
                {{ button2 }}
              </button>
            </a>

            <a
              :href="mylink.python"
              target="_blank"
              rel="noreferrer noopener"
              class="lecture-detail-link1"
            >
              <button class="thqButton lecture-detail-button">
                {{ button3 }}
              </button>
            </a>
          </div>

          <div class="assignment-btn">
            <a
              :href="Problems"
              target="_blank"
              rel="noreferrer noopener"
              class="lecture-detail-link1"
            >
              <button class="thqButton lecture-detail-button">
                {{ button6 }}
              </button>
            </a>
            <a
              :href= "Upload"
              target="_blank"
              rel="noreferrer noopener"
              class="lecture-detail-link1"
            >
              <button class="thqButton lecture-detail-button">
                {{ button7 }}
              </button>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LectureDetail",
  data() {
    return {
      open: false,
      Problems:
        "https://aupedu-my.sharepoint.com/:f:/g/personal/qnguyen_aup_edu/Ett8mGhm3IZHhaPXmw2v80IBzwYxLs9zr0Y0xJm1U_w1GQ?e=EkH2Cj",
      Upload:
        "https://aupedu-my.sharepoint.com/:f:/g/personal/qnguyen_aup_edu/ErHZh_oQ9xhInImh0Ujr4LIBcXuf0wGNSoly19IwYnV91A?e=QxtTWL",
    };
  },
  props: {
    mylink: {},
    lectureTitle: {
      type: String,
      default: "",
    },
    lecture: {
      default: "Lecture 1",
    },

    text2: {
      type: String,
      default: "Lecture Note",
    },
    text4: {
      type: String,
      default: "Watch now!",
    },

    text: {
      type: String,
      default: "Watch Online:",
    },
    text6: {
      type: String,
      default: "Practice",
    },
    text7: {
      type: String,
      default: "Assignment",
    },
    text1: {
      type: String,
      default: "Download",
    },
    sign: {
      type: String,
      default: "+",
    },

    button: {
      type: String,
      default: "Datadesk",
    },
    button1: {
      type: String,
      default: "Excel",
    },
    button2: {
      type: String,
      default: "R",
    },
    button3: {
      type: String,
      default: "Python",
    },
    button4: {
      type: String,
      default: "HTML",
    },
    button5: {
      type: String,
      default: "PDF",
    },
    button6: {
      type: String,
      default: "Problems",
    },
    button7: {
      type: String,
      default: "Upload",
    },
    duration: {
      type: String,
      default: "1 hr 9 min",
    },
  },
};
</script>

<style scoped>
.lecture-detail-container {
  width: 100%;
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}
.lecture-detail-container01 {
  flex: 0 0 auto;
  display: flex;
  width: 100%;
  align-items: flex-start;

  padding-right: var(--dl-space-space-halfunit);
  flex-direction: column;
}
.lecture-detail-container02 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  grid-row-gap: var(--dl-space-space-unit);
  flex-direction: column;
  justify-content: flex-start;
}
.lecture-detail-title {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  transition: 0.3s;
  align-items: center;
  padding-left: 0px;
  padding-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.lecture-detail-text {
  margin-left: var(--dl-space-space-doubleunit);
}
.lecture-detail-text01 {
  margin-right: var(--dl-space-space-doubleunit);
  padding-right: 0px;
}
.lecture-detail-container03 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  grid-gap: var(--dl-space-space-unit);
  align-items: flex-start;
  padding-top: var(--dl-space-space-unit);
  padding-bottom: var(--dl-space-space-unit);
  flex-direction: column;
}
.lecture-detail-container04 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  padding-left: 0px;
  padding-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: var(--dl-color-gray-900);
}
.lecture-detail-text02 {
  margin-left: 4rem;
}

.lecture-detail-container05 {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.lecture-detail-text04 {
  color: red;
  font-size: 14px;
}
.lecture-detail-text05 {
  margin-right: var(--dl-space-space-doubleunit);
}
.lecture-detail-container06 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  padding-left: 0px;
  padding-right: 0px;
  flex-direction: row;
  justify-content: space-between;
}
.lecture-detail-link {
  display: contents;
}
.lecture-detail-watch-now {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  margin-left: var(--dl-space-space-doubleunit);
  padding-left: var(--dl-space-space-halfunit);
  padding-right: var(--dl-space-space-halfunit);
  flex-direction: row;
  justify-content: space-between;
  text-decoration: none;
  background-color: var(--red-cl);
}
.lecture-detail-icon {
  fill: var(--dl-color-gray-white);
  width: 36px;
  height: 36px;
  padding-right: var(--dl-space-space-halfunit);
}
.lecture-detail-text06 {
  color: var(--dl-color-gray-white);
  border-color: rgba(0, 0, 0, 0);
  border-width: 1px;
}
.lecture-detail-link1 {
  display: contents;
}
.lecture-detail-download {
  flex: 0 0 auto;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  text-decoration: none;
  margin-left: 5rem;
}
.lecture-detail-icon2 {
  width: 24px;
  height: 24px;
}
.lecture-detail-text07 {
  padding-left: var(--dl-space-space-halfunit);
}
.lecture-detail-duration {
  margin-left: 31%;
  line-height: 2rem;
}
.lecture-detail-text08 {
  margin-right: var(--dl-space-space-doubleunit);
}
.lecture-detail-container07 {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: flex-start;
}
.lecture-detail-text09 {
  margin-left: var(--dl-space-space-doubleunit);
  margin-right: var(--dl-space-space-doubleunit);
}
.lecture-detail-container08 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
  background-color: var(--dl-color-gray-900);
}
.lecture-detail-text10 {
  margin-left: var(--dl-space-space-doubleunit);
  margin-right: 2.5rem;
}
.lecture-detail-container09 {
  flex: 0 0 auto;
  display: flex;
  align-items: flex-start;
  margin-left: var(--dl-space-space-unit);
  flex-direction: row;
  justify-content: space-between;
  width: 100%;
}
.lecture-detail-button {
  color: var(--dl-color-gray-white);
  border-color: no;
  margin-right: var(--dl-space-space-unit);
  background-color: var(--dl-color-success-700);
  min-width: 5rem;
}

a {
  text-decoration: none;
}
.assignment-btn {
  margin-left: 30%;
  line-height: 2rem;
}
.practice-btn {
  line-height: 2rem;
}
</style>
