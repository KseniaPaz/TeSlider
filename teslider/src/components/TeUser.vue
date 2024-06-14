<template>
    <div class="teachers__item">
      <img :src="require('../assets/img/' + userData.image)" alt="photo">

        
    </div>
</template>

<script>

    export default {
        name: 'TeUser',
        props: 
            {userData: {
                type: Object,
                default() {
                    return {}
                }
              }
            },   
    }

  

</script>

<style lang="scss" scoped>
* {
    margin: 0;
    padding: 0;
}

a {
    text-decoration: none;
}



body {
    font-family: "Jost", sans-serif;
    overflow-x: hidden;
}


summary {
    display: block;
}

summary::-webkit-details-marker {
    display: none;
}

.center {
    padding-left: calc(50% - 610px);
    padding-right: calc(50% - 610px);
}

.teachers {
    padding-top: 16px;
    padding-bottom: 16px;
    padding-left: 180px;

    &__heading {
        font-size: 50px;
        font-weight: 600;
        line-height: 80px;
        text-align: left;
        color: #141024;
    }

    &__box {
        padding-top: 60px;
        display: grid;
        grid-template-columns: repeat(6, 360px);
        gap: 40px;
    }

    &__item {
      display: flex;
      flex-direction: column;
      gap: 20px;
    }

    &__name {
      font-size: 24px;
      font-weight: 600;
      line-height: 38.4px;
      text-align: left;
      color: #141024;
    }

    &__prof {
      font-size: 18px;
      font-weight: 400;
      line-height: 28.8px;
      text-align: left;
      color: #141024B2;
    }

    &__next {
      font-size: 18px;
      font-weight: 400;
      line-height: 28.8px;
      text-align: left;
      color: #D52027;
    }
  }

  .button__box {
    display: flex;
    margin-top: 60px;
    gap: 10px;
    justify-content: flex-end;
  }

  .popup__photo{
    width: 160px;
    height: 222px;
  }

  .popup__heading {
    display: flex;
    gap: 40px
  }

  .popup__ico {
    margin-top: 10px;
    display: flex;
    gap: 10px;
  }

  .popup__details__block {
    display: flex;
    gap: 160px;
    margin: 40px
  }

  .popup__details {
    position: relative;
    padding: 10px;
  }

  .popup__summary {
    padding: 16px;
  }

  .popup__details__box{
    border-top: 1px solid #777779e5;
    width: 776px;
    padding: 6px;
    position: absolute;
    left: 10px;
    display: flex;
    flex-direction: column;
    gap: 10px;
    align-items: flex-start;
  }

  .popup__summary {
    font-size: 20px;
    font-weight: 400;
    line-height: 32px;
    text-align: left;
    color: #141024;
  }

  .popup__details[open] > .popup__summary {
    color: #D52027;
  }

  .popup__text {
    font-size: 20px;
    font-weight: 400;
    line-height: 32px;
    text-align: left;
    color: #141024;
  }

  .popup__title {
    margin-top: 40px;
    margin-bottom: 20px;
    font-size: 24px;
    font-weight: 600;
    line-height: 38.4px;
    color: #141024;
  }

  .popup__text__lorem {
    width: 760px;
    font-size: 20px;
    font-weight: 400;
    line-height: 32px;
    text-align: left;
    color: #141024;
  }



</style>