<script setup>
let topbar_open = true;

// functions
function open_close() {
  if (topbar_open) {
    topbar_open = false;
    document.getElementById("close_topbar_r").style.display = "none";
    document.getElementById("open_topbar_r").style.display = "block";

    document.getElementById("lineadd").style.display = "none";
  } else {
    topbar_open = true;
    document.getElementById("close_topbar_r").style.display = "block";
    document.getElementById("open_topbar_r").style.display = "none";

    document.getElementById("lineadd").style.display = "block";
  }
}

</script>
<template>
  <div id="topbar" class="fxx" style="position: fixed; top: 230px;">
    <div id="close_topbar_r" class="tt_btn_close" @click="open_close"><i class="fa fa-times"></i></div>
    <div id="open_topbar_r" class="tt_btn_open" @click="open_close"><i class="fa fa-plus"></i></div>
    <a id="lineadd" class="tt_img_fixed" target="_blank" href="https://line.me/R/ti/p/@LX789">
      <img src="/public/img/QR_LINEXBET.png">
      <span class="tt_tx_line">
        LINE
      </span>
    </a>
  </div>
</template>