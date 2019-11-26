<template>
  <section>
    <div class="mv-Container">
      <div class="mv-Box">
        <h2>Airbnbホストになって、暮らしをレベルアップ</h2>
        <p>どれくらいの収入が見込めるかチェック</p>
        <InputText></InputText>
        <div class="mv-Box_selectItems">
          <div class="mv-Box_selectWrap">
            <select></select>
          </div>
          <div class="mv-Box_selectWrap">
            <select></select>
          </div>
        </div>
        <p class="mv-Box_priceText">
          <span>¥ 92,673</span>
          <span>月あたり</span>
        </p>
        <ButtonStart>はじめる</ButtonStart>
      </div>
    </div>
  </section>
</template>
<script>
import InputText from '~/components/atoms/InputText'
import ButtonStart from '~/components/atoms/ButtonStart'

export default {
  components: {
    InputText,
    ButtonStart
  }
}
</script>
<style lang="scss" scoped>
.mv {
  &-Container {
    background: url('~assets/images/img_01.jpg') no-repeat;
    background-size: cover;
    width: 100%;
    height: 100%;
    padding: 70px 20px 70px 0;
  }
  &-Box {
    background-color: #fff;
    padding: 20px;
    border-radius: 5px;
    width: 40%;
    margin: 0 0 0 auto;
  }
  &-Box_selectItems {
    margin-top: 10px;
    display: flex;
    justify-content: space-between;
  }
  &-Box_selectWrap:first-child {
    width: 60%;
  }
  &-Box_selectWrap:last-child {
    width: 35%;
  }
  &-Box_selectWrap {
    position: relative;
    select {
      width: 100%;
      height: 40px;
      border: 1px solid gray;
      border-radius: 3px;
      padding: 8px;
      appearance: none;
      background-color: #fff;
    }
    &:after {
      content: '';
      width: 15px;
      height: 15px;
      border: 2px solid;
      border-color: transparent transparent #565656 #565656;
      transform: rotate(-45deg);
      position: absolute;
      top: 8px;
      right: 25px;
    }
  }
  &-Box_priceText {
    span:first-child {
      font-size: 2rem;
      font-weight: 900;
    }
    span:last-child {
      font-size: 0.5rem;
      color: gray;
    }
  }
}
</style>
