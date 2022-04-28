<script setup></script>

<template>
  <section class="login-text-container">
    <div class="login-text-container__item">
      <h4 class="sso-heading">Do you work for Snam?</h4>

      <p class="sso-cta">
        If you are part of the Snam team, log in immediately from here!
      </p>

      <button class="btn-sso">Accedi con le credenziali Snam</button>
    </div>
    <div class="login-text-container__item">
      <h4 class="signup-heading">You are not part of the network yet?</h4>

      <p class="signup-cta">Join us now and become Snaminnovator!</p>

      <button class="btn-signup">Registrati</button>
    </div>
  </section>
</template>

<style scoped lang="scss">
.login-text-container {
  &__item {
    max-width: 100%;
    margin: 0 auto;

    .sso-heading,
    .signup-heading {
      font-size: 24px;
      line-height: 40px;
      text-align: center;
      color: #004c97;
    }
    .sso-cta,
    .signup-cta {
      font-weight: 400;
      font-size: 16px;
      line-height: 24px;
      text-align: center;
      color: #4e5660;
    }
    .btn-sso,
    .btn-signup {
      background: linear-gradient(90deg, #004c97 0%, #2999e7 50%, #00a84a 100%);
      text-align: center;
      padding: 11px 20px;
      color: #fff;
      background-clip: text;
      -webkit-background-clip: text;
      -webkit-text-fill-color: rgba(255, 255, 255, 0.001);
      transition: 256ms all;
      position: relative;
      cursor: pointer;
      background-size: 200% 100%;
      background-position: right center;
      z-index: 1;
      -webkit-border-radius: 100px;
      -moz-border-radius: 100px;
      -ms-border-radius: 100px;
      border-radius: 100px;
      font-size: 16px;
      font-weight: 700;

      &::before {
        content: '';
        position: absolute;
        top: -1px;
        bottom: -1px;
        left: -1px;
        right: -1px;
        background: linear-gradient(
          90deg,
          #004c97 0%,
          #2999e7 50%,
          #00a84a 100%
        );
        transition: 256ms all;
        z-index: -1;
        background-size: 200% 100%;
        background-position: right center;
        -webkit-border-radius: 100px;
        -moz-border-radius: 100px;
        -ms-border-radius: 100px;
        border-radius: 100px;
      }

      &::after {
        background: #fff;
        content: '';
        position: absolute;
        top: 0px;
        bottom: 0px;
        left: 0px;
        right: 0px;
        z-index: -1;
        -webkit-border-radius: 100px;
        -moz-border-radius: 100px;
        -ms-border-radius: 100px;
        border-radius: 100px;
      }

      &:hover::before {
        opacity: 50%;
        top: 0px;
        right: 0px;
        bottom: 0px;
        left: 0px;
      }
      &:hover::after {
        color: white;
      }
    }
  }
}
</style>
