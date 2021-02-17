<template>
  <div class="footer">
      <a href=""><img src="../assets/Unionlogo.png" alt="" class="footer__logo"></a>
      <ul class="footer__list">
          <li class="footer__item"><a href="" class="footer__link">Why PM</a></li>
          <li class="footer__item"><a href="" class="footer__link">Our products</a></li>
          <li class="footer__item"><a href="" class="footer__link">Dermatologist consultation</a></li>
          <li class="footer__item">
              <ul class="footer__contacts">
                  <li class="footer__contact-item"><a href="" class="footer__link">Contacts</a></li>
                  <li class="footer__contact-item"><a href="" class="footer__link">+ 38 (063) 4376524</a></li>
                  <li class="footer__contact-item"><a href="" class="footer__link">email@gmail.com</a></li>
              </ul>
          </li>
      </ul>
  </div>
</template>

<script>
export default {

}
</script>

<style lang='scss'>
    .footer{
        padding: 82px 0 103px;
        background-color: $black;
        @include flex(center, center, row);
        &__logo{
            margin-right: 80px;
        }
        &__list{
            @include flex(flex-start, center, row);
        }
        &__item{
            &:not(last-child){
                margin-right: 70px;
            }
        }
        &__link{
            @include text($H80, 500, $white){
                text-decoration: none;
            };
        }
        &__contact-item{
            &:not(last-child){
                margin-bottom: 11px;
            }
        }
    }
</style>