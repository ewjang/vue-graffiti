<template>
  <div>
    <div
      class="btnGrp"
      v-for="btnTest in btnTests"
      :key="btnTest.equipId"
      :src="btnTest.equipType"
    >
      <button class="indiBtn" @click="btnClick(btnTest)">
        {{ btnTest.equipNm }}
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ekolas-ekdoc-manage",
  props: {},
  data() {
    return {
      btnTests: [],
    };
  },
  watch: {},
  beforeCreate() {},
  created() {},
  beforeMount() {
    this.init();
  },
  mounted() {
    this.btnTests = [
      { equipId: 0, equipNm: "sq0", equipType: "0cd" },
      { equipId: 1, equipNm: "sq1", equipType: "1cd" },
      { equipId: 2, equipNm: "sq2", equipType: "2cd" },
      { equipId: 3, equipNm: "sq3", equipType: "3cd" },
      { equipId: 4, equipNm: "sq4", equipType: "4cd" },
      { equipId: 5, equipNm: "sq5", equipType: "5cd" },
      { equipId: 6, equipNm: "sq6", equipType: "6cd" },
      { equipId: 7, equipNm: "sq7", equipType: "7cd" },
      { equipId: 8, equipNm: "sq8", equipType: "8cd" },
      { equipId: 9, equipNm: "sq9", equipType: "9cd" },
      { equipId: 10, equipNm: "sq10", equipType: "10cd" },
      { equipId: 11, equipNm: "sq11", equipType: "11cd" },
      { equipId: 12, equipNm: "sq12", equipType: "12cd" },
      { equipId: 13, equipNm: "sq13", equipType: "13cd" },
      { equipId: 14, equipNm: "sq14", equipType: "14cd" },
      { equipId: 15, equipNm: "sq15", equipType: "15cd" },
      { equipId: 16, equipNm: "sq16", equipType: "16cd" },
    ];
  },
  beforeDestroy() {},
  methods: {
    init() {},
    btnClick(event) {
      console.log(event);
    },
  },
};
</script>

<style>
.btnGrp {
  float: left;
}
.indiBtn {
  margin-right: 5px;
  margin-bottom: 5px;
  width: 100px;
  height: 120px;
}
</style>
