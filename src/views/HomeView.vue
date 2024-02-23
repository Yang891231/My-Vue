<script setup>

</script>

<template>
  <main>
    <div class="my-all w-100 vh-100 d-flex flex-xl-row flex-column">
      <div class="nav bg-dark flex-shrink-0 d-flex flex-column align-items-center">
        <ul class="nav-pills w-25 d-sm-none mt-3 me-auto">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">
              <div id="line-1" class="line bg-body-secondary w-100 mx-auto"></div>
              <div id="line-2" class="line bg-body-secondary w-100 mx-auto mt-2"></div>
              <div id="line-3" class="line bg-body-secondary w-100 mx-auto mt-2"></div>
            </a>
            <ul class="dropdown-menu">
              <li><a target="_blank" class="dropdown-item btn btn-secondary" href="https://www.youtube.com/">YouTube</a>
              </li>
              <li><a target="_blank" class="dropdown-item btn btn-secondary"
                  href="https://www.google.com.tw/?hl=zh_TW">Google</a></li>
              <li><a target="_blank" class="dropdown-item btn btn-secondary "
                  href="https://www.google.com/intl/zh-TW_tw/gmail/about/">Gmail</a></li>
            </ul>
          </li>
        </ul>
        <div class="logo mt-xl-5 mb-xl-3 mt-2 me-auto m-auto"></div>
        <div class="nav-all-link d-sm-flex flex-row flex-xl-column mt-xl-5 mt-4 ms-sm-5 mx-xl-auto d-none gap-3">
          <a target="_blank" href="https://www.youtube.com/" class="link fs-3 text-white p-2 mt-xl-5 ">YouTube</a>
          <a target="_blank" href="https://www.google.com.tw/?hl=zh_TW"
            class="link fs-3 text-white p-2 mt-xl-3 ">Google</a>
          <a target="_blank" href="https://www.google.com/intl/zh-TW_tw/gmail/about/"
            class="link fs-3 text-white p-2 mt-xl-3 ">Gmail</a>
        </div>
      </div>
      <div class="my-container flex-grow-1 bg-body-secondary d-flex justify-content-center align-items-center">
        <div class="content">
          <div class="all-img h-100 d-flex flex-wrap">
            <div class="col-12 col-sm-12 col-xxl img" style="background-image: url(./img/cat1.jpg);">
            </div>
            <div class="col-12 col-sm col-xxl img ms-xxl-2 mt-sm-2 me-sm-1 mt-xxl-0
                    me-xxl-0" style="background-image: url(./img/cat2.jpg);"></div>
            <div class="col-12 col-sm col-xxl img mt-sm-2 ms-sm-1 mt-xxl-0 ms-xxl-2"
              style="background-image: url(./img/cat3.jpg);"></div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
