<template>
<div v-if="show">
  <div class="container">
      <div id="title">Christmas Q25</div>
      <div class="subtitle">- 당신의 1년을 정리하는 25개의 질문 -</div>
      <div id="logo">로고</div>
      <div><button @click="introBtnOn" type="button" class="btn" id="introductionBtn">소개</button></div>
      <div><button type="button" onclick="" class="btn">시작하기</button></div>
      <div><button type="button" onclick="" class="btn">비밀번호 찾기</button></div>
      <div style="color: white;">teamname</div>
  </div>
</div>

<div v-else>
  <div><button @click="introBtnOn" type="button" id="backBtn">Back</button></div>
  <div class="container">    
      <div id="title">Christmas Q25</div>
      <div class="subtitle">- 당신의 1년을 정리하는 25개의 질문 -</div>
      <div id="introductionBox">
          <p>Christmas Q25는 12월 1일부터 12월 25일 크리스마스까지
          1년을 돌아볼 수 있는 질문들을 매일 하나씩 제공합니다.</p>
          <p>여러분들은 각 질문에 대한 답변을 작성하며 1년을 되돌아보고, 정리할 수 있을 것입니다.</p>
          <p>Christmas Q25가 1년동안의 소중했던 추억, 행복했던 기억, 고마웠던 사람을 떠올리게 하는
              따뜻한 매개체가 되길 바라며
          </p>
          <p>모든 사용자분들의 행복한 연말을 기원합니다.</p>
      </div>
      <div><button @click="introBtnOn" type="button" class="btn" id="closeBtn">닫기</button></div>
  </div>
</div>
</template>

<script>
export default {
  name: 'App',
  components: {
  },
  data(){
    return {
      show : true,
    }
  },
  methods: {
    introBtnOn() {
      this.show = !this.show;
    }
  },
}


</script>

<style>
@font-face {
    font-family: 'NanumSquareRound';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_two@1.0/NanumSquareRound.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}

@import url('https://fonts.googleapis.com/css2?family=Sorts+Mill+Goudy&display=swap');

.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #920000;
    width: 360px; height: 640px;
    margin: 0 auto;
}

.btn {
    margin: 7px;
    background-color: white;
    border: none;
    border-radius: 3px;
    width: 120px; height: 30px;
    cursor: pointer;

    font-weight: bold;
}

#title {
    color: #FFF500;
    font-family: 'Sorts Mill Goudy', serif;
    font-size: 50px;
    margin-top: 50px;
}

#logo {
    color: black;
    width: 50px;
    padding: 60px;
    border: 1px solid black;
    margin: 40px;
    padding-top: 70px;
    padding-bottom: 70px;
    text-align : center;

    background-color: white;
}

#introductionBox {
    border: 1px solid black;
    width: 300px;
    background-color: white;
    margin: 25px;
}

#Registration {
    color: black;
    width: 50px;
    padding: 60px;
    border: 1px solid black;
    margin: 40px;
    text-align: center;

    background-color: white;
}

#backBtn {
    background-color:rgba(0,0,0,0);
    color: #0D86FE;
    font-weight: bold;
    border-color: transparent;
    border: none;
    cursor: pointer;
}

.subtitle {
    color: white;
}

#password {
    width: 170px; height: 30px;
    border-radius: 3px;
    border: none;
    margin: 5px;
    text-align: center;
}

body {
    font-family: 'NanumSquareRound';
}

#usermail {
    text-decoration-line: underline;
    color: blue;
    text-align: center;
}
</style>
