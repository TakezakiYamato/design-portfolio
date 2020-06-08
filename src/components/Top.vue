<template>
  <div id="top">
    <div class="top-contents">
      <!-- テキスト中心の左のコンテンツ部分 -->
      <div class="top-text-contents">
        <div class="top-text">
          <h1>Make a difference in the world<br>by using power of design</h1>
          <h3>Portfolio of Yamato Takezaki</h3>
          <h3>UI・UX designer / Web Design / Web Development</h3>
        </div>
        <div class="top-sns-icon">
          <div/>
          <div class="sns-icon">
            <img src="../assets/twitter.svg">
            <img src="../assets/facebook.svg">
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
   padding: 8px;
}
.top-text h3 {
   color: rgba(32, 42, 147, 0.75);
   font-family: 'Lato', sans-serif;
   padding: 0px 8px 2px 8px;
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
.sns-icon img {
  padding: 0 10px;
}
.profile-picture img {
  width: 250px;
  height: 250px;
}
</style>
