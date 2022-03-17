<template>
  <div>
    <ul
      class="
        nav nav-tabs
        flex flex-row flex-nowrap
        list-none
        border-b-0
        mb-4
        overflow-scroll
        pl-[20px]
        pr-[20px]
        rounded-[12px]
      "
      id="tabs"
      role="tablist"
    >
      <li class="flex-auto text-center" role="presentation">
        <div
          class="
            w-full
            block
            font-bold
            text-[14px]
            min-w-[160px]
            text-[#319795]
            border-[1px] border-[#CBD5E0]
            px-6
            py-2
            my-2
            hover:border-transparent
            rounded-l-[12px]
            active
            bg-white
          "
          :class="tab === 'tab1' && 'bg-[#81E6D9] text-[#E6FFFA] border-[#81E6D9]'"
          id="tab1"
          @click="selectTab('tab1')"
          >Arbeitnehmer</div
        >
      </li>
      <li class="flex-auto text-center" role="presentation">
        <div
          class="
            w-full
            block
            font-bold
            text-[14px]
            min-w-[160px]
            text-[#319795]
            border-[1px] border-[#CBD5E0]
            px-6
            py-2
            my-2
            hover:border-transparent
            bg-white
          "
          :class="tab === 'tab2' && 'bg-[#81E6D9] text-[#E6FFFA] border-[#81E6D9]'"
          id="tab2"
          @click="selectTab('tab2')"
          >Arbeitgeber</div
        >
      </li>
      <li class="flex-auto text-center" role="presentation">
        <div
          class="
            w-full
            block
            font-bold
            text-[14px]
            min-w-[160px]
            text-[#319795]
            border-[1px] border-[#CBD5E0]
            px-6
            py-2
            my-2
            hover:border-transparent rounded-r-[12px]
            bg-white
          "
          :class="tab === 'tab3' && 'bg-[#81E6D9] text-[#E6FFFA] border-[#81E6D9]'"
          id="tab3"
          @click="selectTab('tab3')"
          >Temporärbüro</div
        >
      </li>
    </ul>
  </div>
</template>

<style scoped>
#tabs::-webkit-scrollbar {
  display: none;
}
</style>

<script>
export default {
    data: function () {
        return {
            tab: 'tab1',
        }
    },
    methods: {
        selectTab: function (key) {
            this.tab = key;
            this.$emit('handleChangeTab', key);
            const element = document.getElementById('tabs');
            if (key === 'tab1') {
                element.scroll({
                    top: 0,
                    left: 0,
                    behavior: 'smooth'
                });
            }
            if (key === 'tab2') {
                element.scroll({
                    top: 0,
                    left: 75,
                    behavior: 'smooth'
                });
            }
            if (key === 'tab3') {
                element.scroll({
                    top: 0,
                    left: 200,
                    behavior: 'smooth'
                });
            }
        }
    }
}
</script>