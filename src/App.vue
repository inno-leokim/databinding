<template>
  <div> <!-- 입력 -->
    <h2>{{ title }}</h2>
    <input v-model="title">
  </div>
  <div> <!-- 체크박스 -->
    <h2>웹툰</h2>
    <div>
      <input type="checkbox" id="프롬스타" value="프롬스타" v-model="checkWebtoons" />
      <label for="프롬스타">프롬스타</label>
      <input type="checkbox" id="햄스터와그녀" value="햄스터와그녀" v-model="checkWebtoons" />
      <label for="햄스터와그녀">햄스터와그녀</label>
      <input type="checkbox" id="위대한로맨스" value="위대한로맨스" v-model="checkWebtoons" />
      <label for="위대한로맨스">위대한로맨스</label>
      <input type="checkbox" id="아귀" value="아귀" v-model="checkWebtoons" />
      <label for="아귀">아귀</label>
      <br>
      <span>찜한 웹툰: {{ checkWebtoons }}</span>
    </div>
  </div>
  <div> <!-- 라디오 버튼-->
    <h2>성별</h2>
    <input type="radio" id="male" value="male" v-model="gender">
    <label for="male">남</label>
    <br>
    <input type="radio" id="female" value="female" v-model="gender">
    <label for="female">여</label>
    <br>
    <span>당신의 성별을 알려주세요: {{ gender }}</span>
  </div>
  <div> <!-- 셀렉트 박스 -->
    <h2>선호 장르</h2>
    <select v-model="category" name="" id="">
      <option disabled value>선택해주세요</option>
      <option>로맨스</option>
      <option>호러</option>
      <option>스릴서</option>
    </select>
    <br>
    <span>선택: {{ category }}</span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "",
      checkWebtoons: [],
      gender: "",
      category: ""
    };
  }
};
</script>

<style>
</style>
