<template>
  <footer>
    <div class="footer-contents">
      <div class="sns-icon">
        <div class="icon">
          <a href="https://www.facebook.com/profile.php?id=100022957357074">
            <font-awesome-icon :icon="['fab', 'facebook-f']" class="facebook fa-lg" style="color:darkblue;"/>
          </a>
        </div>
        <div class="icon">
          <a href="https://twitter.com/yamantis_">
            <font-awesome-icon :icon="['fab', 'twitter']" class="twitter fa-lg" style="color:darkblue;" />
          </a>
        </div>
      </div>
      <div class="footer-title">
        <h4>Yamato Takezaki</h4>
      </div>
      <div class="copyright">
        <p>©︎ 2020 Yamato Takezaki</p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  width: 100%;
  display: flex;
  justify-content: center;
}
.footer-contents {
  margin-top: 72px;
  padding: 40px 8px;
  width: 80%;
  height: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-top: 3px solid rgba(32, 42, 147, 0.90);
}
.copyright p {
  padding-top: 12px;
  font-size: 12px;
  letter-spacing: 0.05em;
  color: #777777;
}
.sns-icon {
  display: flex;
  margin-bottom: 10px;
}
.icon {
  border: 2px solid rgba(32, 42, 147, 0.95);
  border-radius: 50%;
  width: 46px;
  height: 46px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-right: 18px;
}
.facebook {
  margin-right: 2px;
}
a {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}
</style>