<template>
  <div id="top">
    <div class="top-contents">
      <!-- テキスト中心の左のコンテンツ部分 -->
      <div class="top-text-contents">
        <div class="top-text">
          <h1>Make a difference in the world<br>by using power of design</h1>
          <div class="discript">
            <p class>Portfolio of Yamato Takezaki</p>
            <p>UI・UX designer / Web Design / Web Development</p>
          </div>
        </div>
        <div class="top-sns-icon">
          <div/>
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
        </div>
      </div>
      <div class="profile-picture">
        <img src="@/assets/profilePicture.jpg" >
      </div>
    </div>
  </div>
</template>
<style scoped>
#top {
  width: 100%;
  height: 100%;
  /* 子要素をフレックスボックス化 */
  display: flex;
  /* 横中央に寄せる */
  justify-content: center;
  /* たて中央に寄セル */
  align-items: center;
}
.top-contents {
  width: 80%;
  height: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 72px 0px;
}
.top-text h1 {
   font-family: 'Lato', sans-serif;
   font-size: 48px;
   padding: 8px;
   line-height: 1.3;
   letter-spacing: 0.03em;
}
.discript {
  margin-top: 10px;
}
.top-text p {
   color: rgba(32, 42, 147, 0.75);
   font-family: 'Lato', sans-serif;
   font-size: 22px;
   padding: 0px 8px 0px 8px;
   letter-spacing: 0.03em;
   font-weight: 700;
   margin: 0px;
}
.top-text-contents {
  float:left
}
.top-sns-icon {
  margin-top: 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
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
.profile-picture img {
  width: 250px;
  height: 250px;
}
a {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}
</style>
