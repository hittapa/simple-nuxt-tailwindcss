<template>
  <div class="max-w-full pb-[100px] text-center">
    <div class="w-full pt-[80px] bg-gradient-to-b from-[#EBF4FF] to-[#E6FFFA]">
      <p
        class="
          text-[#2D3748] text-[42px]
          font-normal
          pr-16
          pl-16
          pb-6
          leading-tight
          font-['lato']
        "
      >
        Deine Job website
      </p>
      <img
        src="~/assets/img/undraw_agreement_aajr@2x.png"
        class="w-full h-auto object-contain"
      />
    </div>
    <div class="w-full pt-[20px]">
      <Tabs @handleChangeTab="handleChangeTab" />
    </div>
    <div v-if="tab === 'tab1'" class="w-full fade">
      <div class="w-full px-[40px] py-2">
        <p class="font-medium text-[21px] text-[#4A5568] text-center">
          Drei einfache Schritte
        </p>
        <p class="font-medium text-[21px] text-[#4A5568] text-center">
          zu deinem neuen Job
        </p>
        <div class="w-full py-2 flex flex-row justify-end">
          <img
            src="~/assets/img/undraw_Profile_data_re_v81r@2x.png"
            class="w-[75%] h-auto object-contain z-10"
          />
        </div>
      </div>
      <div class="w-full px-2 flex flex-row justify-start items-center -mt-[90px] relative">
        <div class="absolute w-[174px] h-[208px] bg-[#F7FAFC88] rounded-[50%] -left-4 -bottom-4 -z-10"></div>
        <p class="text-[130px] text-[#718096] z-10">1. <span class="text-[16px]">Erstellen dein Lebenslauf</span></p>
      </div>
      <div id="section-1-2" class="w-full py-4 z-10">
        <div class="w-full pr-2 pl-12 flex flex-row justify-start items-center -mt-[40px]">
          <p class="text-[130px] text-[#718096]">2. <span class="text-[16px]">Erstellen dein Lebenslauf</span></p>        
        </div>
        <div class="w-full pl-[40px] pr-0 -mt-[20px]">
          <div class="w-full flex flex-row justify-center">
            <img
              src="~/assets/img/undraw_task_31wc@2x.png"
              class="w-[60%] h-auto object-contain"
            />
          </div>
        </div>
      </div>
      <div class="w-full py-4">
        <div class="w-full pr-2 pl-16 flex flex-row justify-start items-center -mt-[40px]">
          <p class="text-[130px] text-[#718096]">3.</p>
          <p class="text-[16px] text-[#718096] text-left ml-2">Mit nur einem Klick bewerben</p>
        </div>
        <div class="w-full pl-[40px] pr-2 -mt-[20px]">
          <div class="w-full flex flex-row justify-end">
            <img
              src="~/assets/img/undraw_personal_file_222m@2x.png"
              class="w-[80%] h-auto object-contain"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- Tab 2 -->
    <div v-if="tab === 'tab2'" class="w-full fade">
      <div class="w-full px-[40px] py-2">
        <p class="font-medium text-[21px] text-[#4A5568] text-center">
          Drei einfache Schritte
        </p>
        <p class="font-medium text-[21px] text-[#4A5568] text-center">
          zu deinem neuen Mitarbeiter
        </p>
        <div class="w-full py-2 flex flex-row justify-end">
          <img
            src="~/assets/img/undraw_Profile_data_re_v81r@2x.png"
            class="w-[75%] h-auto object-contain z-10"
          />
        </div>
      </div>
      <div class="w-full px-2 flex flex-row justify-start items-center -mt-[90px] relative">
        <div class="absolute w-[174px] h-[208px] bg-[#F7FAFC88] rounded-[50%] -left-4 -bottom-4 -z-10"></div>
        <p class="text-[130px] text-[#718096] z-10 pr-4">1.</p>
        <span class="text-[16px] text-[#718096] z-10 px-6 text-left mt-10">Erstellen dein Unternehmensprofil</span>
      </div>
      <div id="section-1-2" class="w-full py-4 z-10">
        <div class="w-full pr-2 pl-12 flex flex-row justify-start items-center -mt-[40px]">
          <p class="text-[130px] text-[#718096]">2. <span class="text-[16px]">Erstellen dein Lebenslauf</span></p>        
        </div>
        <div class="w-full pl-[40px] pr-0 -mt-[20px]">
          <div class="w-full flex flex-row justify-center">
            <img
              src="~/assets/img/undraw_about_me_wa29@2x.png"
              class="w-[80%] h-auto object-contain -mt-16"
            />
          </div>
        </div>
      </div>
      <div class="w-full py-4">
        <div class="w-full pr-2 pl-16 flex flex-row justify-start items-center -mt-[40px]">
          <p class="text-[130px] text-[#718096]">3.</p>
          <p class="text-[16px] text-[#718096] text-left ml-2">Wähle deinen neuen Mitarbeiter aus</p>
        </div>
        <div class="w-full px-2 -mt-[20px]">
          <div class="w-full flex flex-row justify-center px-4">
            <img
              src="~/assets/img/undraw_swipe_profiles1_i6mr@2x.png"
              class="w-[80%] h-auto object-contain"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- Tab 3 -->
    <div v-if="tab === 'tab3'" class="w-full fade">
      <div class="w-full px-[40px] py-2">
        <p class="font-medium text-[21px] text-[#4A5568] text-center">
          Drei einfache Schritte
        </p>
        <p class="font-medium text-[21px] text-[#4A5568] text-center">
          zur Vermittlung neuer Mitarbeiter
        </p>
        <div class="w-full py-2 flex flex-row justify-end">
          <img
            src="~/assets/img/undraw_Profile_data_re_v81r@2x.png"
            class="w-[75%] h-auto object-contain z-10"
          />
        </div>
      </div>
      <div class="w-full px-2 flex flex-row justify-start items-center -mt-[90px] relative">
        <div class="absolute w-[174px] h-[208px] bg-[#F7FAFC88] rounded-[50%] -left-4 -bottom-4 -z-10"></div>
        <p class="text-[130px] text-[#718096] z-10 pr-4">1.</p>
        <span class="text-[16px] text-[#718096] z-10 px-6 text-left mt-10">Erstellen dein Unternehmensprofil</span>
      </div>
      <div id="section-1-2" class="w-full py-4 z-10">
        <div class="w-full pr-2 pl-12 flex flex-row justify-start items-center -mt-[40px]">
          <p class="text-[130px] text-[#718096]">2.</p>
          <p class="text-[16px] text-[#718096] text-left ml-2 mt-8">Erhalte Vermittlungs- angebot von Arbeitgeber</p>
        </div>
        <div class="w-full pl-8 pr-8">
          <div class="w-full flex flex-row justify-end">
            <img
              src="~/assets/img/undraw_job_offers_kw5d@2x.png"
              class="w-[70%] h-auto object-contain -mt-8"
            />
          </div>
        </div>
      </div>
      <div class="w-full py-4">
        <div class="w-full pr-2 pl-16 flex flex-row justify-start items-center -mt-[40px]">
          <p class="text-[130px] text-[#718096]">3.</p>
          <p class="text-[16px] text-[#718096] text-left ml-4 mr-4 mt-6">Vermittlung nach Provision oder Stundenlohn</p>
        </div>
        <div class="w-full px-2 -mt-[20px]">
          <div class="w-full flex flex-row justify-center px-4">
            <img
              src="~/assets/img/undraw_business_deal_cpi9@2x.png"
              class="w-[80%] h-auto object-contain"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Tabs from "../components/Tabs.vue";
export default {
  name: "IndexPage",
  components: {
    Tabs,
  },
  data: function () {
    return {
      tab: "tab3",
    };
  },
  methods: {
    handleChangeTab: function (params) {
      this.tab = params;
    },
  },
};
</script>

<style scoped>
  #section-1-2 {
    background: transparent linear-gradient(134deg, #E6FFFA 0%, #EBF4FF 100%) 0% 0% no-repeat padding-box;
  }
  .fade {
    animation: fade 1s;

  }
  @keyframes fade {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }
</style>