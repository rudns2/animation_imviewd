<template>
    <div>
      <div class="ani_img_wrap">
        <ul>
          <li v-for="item in animation" :key="item">
            <h1>{{ item.aniName }}</h1>
            <img :src="require(`@/assets/img/${item.aniImg}`)" alt="">
            <span class="clear_tag" v-if="item.isClear">clear</span>
          </li>
        </ul>
      </div>
    </div>
</template>
<script>
  export default {
    data() {
      return {
        animation: [{
            aniName: '어둠의 실력자가 되고싶어서!',
            aniImg: 'ani1.png',
            isClear : 'true'
          },
          {
            aniName: '터무니없는 스킬로 이세계방랑밥',
            aniImg: 'ani2.jpg',
            isClear : 'true'
          },
          {
            aniName: '해골기사님은 지금 이세계 모험중',
            aniImg: 'ani3.jpg',
            isClear : 'true'
          },
          {
            aniName: '블루록',
            aniImg: 'ani4.jpg',
            isClear : 'true'
          },
          {
            aniName: '현실주의 용사의 왕국 재건기',
            aniImg: 'ani5.jpg',
            isClear : 'true'
          },
          {
            aniName: '봇치 더 락',
            aniImg: 'ani6.jpg',
            isClear : 'true'
          },
          {
            aniName: '하이큐!',
            aniImg: 'ani7.jpg',
            isClear : 'true'
          },
        ]
      }
    }
  }
</script>
<style scoped>
  .ani_img_wrap {
    padding: 0 2rem;
  }

  .ani_img_wrap ul {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    gap: 10px;

  }

  .ani_img_wrap ul li {
    width: 24%;
    margin-top: 15px;
    position : relative;
  }

  .ani_img_wrap ul li h1 {
    font-size: 18px;
    color : #222;
    text-shadow: 1px 2px 1px #222;
  }

  .ani_img_wrap ul li img {
    width: 100%;
    height: 100%;
  }
  .clear_tag{
    font-size : 20px;
    padding : 10px;
    background-color: rgb(0, 208, 0);
    color : #eee;
    border-radius : 5px;
    position : absolute;
    bottom: -25px;
    right: 0;
  }
</style>