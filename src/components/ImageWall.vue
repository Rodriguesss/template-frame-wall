<template>
  <div>
    <!--<vue-image-wall :link-images="images"></vue-image-wall>-->
    <br />
    <div id="image-wall-wrapper">
      <div id="image-wall">
        <div id="container_images">
          <div id="image-frame" style="width: 18%" class="frame-format-box" :class="widthDiv">
            <img
              class="frame-box image-format"
              @mousemove="alterSize(1)"
              src="https://uhdwallpapers.org/uploads/converted/19/08/03/huawei-mediapad-m6-stock-wallpaper-1080x1920_666874-mm-90.jpg"
            />
          </div>

          <div id="image-frame" style="width: 22%" class="frame-format-box" :class="widthDiv">
            <img
              class="frame-box image-format"
              @mousemove="alterSize(2)"
              src="https://s1.1zoom.me/b3556/124/Texture_Multicolor_526935_1080x1920.jpg"
            />
          </div>

          <div id="image-frame" style="width: 22%" class="frame-format-box" :class="widthDiv">
            <img
              class="frame-box image-format"
              @mousemove="alterSize(3)"
              src="https://image.winudf.com/v2/image/aGlnaGxhcmdlLmhkLndhbGxwYXBlci5waG90b3Nfc2NyZWVuXzBfMTUzNDgwNjc4NV8wOTg/screen-0.jpg?fakeurl=1&type=.jpg"
            />
          </div>

          <div id="image-frame" style="width: 20%" class="frame-format-box" :class="widthDiv">
            <img
              class="frame-box image-format"
              @mousemove="alterSize(4)"
              src="https://wallpaperaccess.com/full/889705.jpg"
            />
          </div>

          <div id="image-frame" style="width: 20%" class="frame-format-box" :class="widthDiv">
            <img
              class="frame-box image-format"
              @mousemove="alterSize(5)"
              src="https://i.pinimg.com/originals/00/5c/a7/005ca765038679e314b2df606eb1e0dd.jpg"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
#image-wall-wrapper {
  display: block;
}

#image-wall {
  overflow: hidden;
  box-sizing: border-box;
  border: 2px solid black;
  height: 350px;
  border-radius: 30px;
  background-color: black;
}

#container_images {
  white-space: nowrap;
  position: relative;
  left: -15px;
}

#image-frame {
  box-sizing: content-box;
  overflow: hidden;
  display: inline-block;
  width: 20%;
  transform: skew(-10deg);
  border-right: 3px solid black;
  height: 350px;
  transition: all 250ms ease 0s;
}

.frame-box {
  display: block;
  position: relative;
  object-fit: cover;
  height: 100%;
}

.image-format {
  width: 120%;
  left: -12%;
  transform: skew(2deg);
  transition: all 250ms ease 0s;
}

#image-frame:hover {
  width: 40% !important;
}

.image-format:hover {
    width: 120% !important;
}
</style>