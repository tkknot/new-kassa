<template>
  <div>

    <header class="w-100" id="header">
      <div id="header-up">
        <div class="h-100 w-100 d-sm-flex">
          <div class="w-50 h-sm-100 h-xs-25" id="ccbox">
            <span id="catchcopy" class="pl-lg-7 pl-sm-16 text-white">
              one step ahead in relaxation
            </span>
          </div>
          <div class="h-100 m-auto" id="logo">
            <v-img src="/img/logo-new.jpg" class="h-100" max-width="1000"></v-img>
          </div>
        </div>
      </div>
      
      <nav id="header-bottom">
        <ul class="d-flex w-100 p-0" id="items">
          <i class="fas fa-bars fa-2x" id="hamburger">
          </i>
          <li class="h-100 text-center h5" id="item">
            <div class="w-100 h-100" id="menu-kassa">
                <v-card color="rgba(255,193,193,0.6)" class="text-white">
                  かっさとは
                </v-card>
              </div>
          </li>
          <li class="h-100 text-center h5" id="item">
            <div class="w-100 h-100" id="menu-salon">
              <v-card color="rgba(255,193,193,0.6)" class="text-white">
                当サロン
              </v-card>
            </div>
          </li>

          <li class="h-100 text-center h5" id="item">
            <div class="w-100 h-100" id="menu-therapist">
            <v-card color="rgba(255,193,193,0.6)" class="text-white">
                セラピスト
              </v-card>
            </div>
          </li>

          <li class="h-100 text-center h5" id="item">
            <div class="w-100 h-100">
              <div class="w-100 h-100" id="menu-treatment">
                <v-card color="rgba(255,193,193,0.6)" class="text-white">
                  施術について
                </v-card>
              </div>
            </div>
          </li>
          
          <li class="h-100 text-center h5" id="item">
            <div class="w-100 h-100" id="menu-notification">
            <v-card color="rgba(255,193,193,0.6)" class="text-white">
                お知らせ
              </v-card>
            </div>
          </li>
        </ul>
      </nav>
    </header>
    
    <v-main>
      <h1 class="text-center h2" id="title">刮痧について</h1>
      
      <div class="container" id="text-zone">
        
        <div class="row">
          
          <div class="col-lg-5 w-75 mx-auto">
            <img src="img/desc-about-kassa.JPG" alt="" srcset="" class="d-block w-100 h-100 rounded">
          </div>
          
          <div class="col-lg-7 w-75 m-auto">
            <p><ruby><rb>刮痧</rb><rp>（</rp><rt>※グアシャ</rt><rp>）</rp></ruby>は中国で古くから伝わる、
              <ruby><rb>東洋医学</rb><rt>※</rt></ruby>を基礎とした治療法です。</p>
              <p>これを日本式にアレンジし女性の優しさ・柔らかさをイメージした<br>
                ひらがな表記「かっさ」は、「かっさの名付け親」島田 <ruby><rb>淑子</rb><rp>（</rp><rt>すみこ</rt><rp>）</rp></ruby>先生考案の<br>
                オリジナルメソッドです。</p>
                <p>気、血、水の通り道（経路）に圧を加えて滞りを流し、<br>
                  精神面・肉体面にアプローチできる、リラクゼーショントリートメントです。</p>
                  <p class="h7 font-weight-light">
                  <ruby><rb>刮</rb><rt>※かつ</rt></ruby>…けずる・こする<br>
                  <ruby><rb>痧</rb><rt>さ</rt></ruby>…<ruby><rb>瘀血</rb><rp>（</rp><rt>おけつ</rt><rp>）</rp></ruby>（滞って流れなくなった血液の毒）<br>
                  <ruby><rb>東洋医学</rb><rt>※</rt></ruby>：中国の伝統医学。不調の原因をパーソナルに見立ててアプローチします。
              </p>
            </div>
            
          </div>
          
        </div>
      </v-main>
      
        <v-bottom-navigation :value="value" grow color="pink" :height="breakPoint">
          <div class="container">
            <div class="row">
              <div class="col-sm-4 mr-0">
                <v-card :width="cardWidthBreakPoint" :height="cardBreakPoint" class="pt-6 mx-auto">
                  <v-card-text class="text--h7">
                    〒250-0051<br>
                    神奈川県小田原市北ノ窪48-1<br>
                    メゾンメルベーユ102<br>
                    電話番号：080-5880-9076<br>
                    メール：kassa.yuu@gmail.com
                  </v-card-text>
                  <div class="container">
                    <div class="row">
                      <div class="col-4 text-center">
                        <a href="https://www.instagram.com/kassa.yuu/">
                          <i class="fab fa-instagram fa-4x" style="color: #D93177;"></i>
                        </a>
                      </div>
                      <div class="col-4 text-center">
                        <a
                          href="https://ja-jp.facebook.com/pages/category/Health-Beauty/%E3%81%8B%E3%81%A3%E3%81%95-yuu-146418565810698/">
                          <i class="fab fa-facebook-square fa-4x" style="color: #3B5998;"></i>
                        </a>
                      </div>
                      <div class="col-4">
                        <a href="https://ameblo.jp/yuu-kassa/">
                          <p class="text-success">Ameba</p>
                        </a>
                      </div>
                    </div>
                  </div>
                </v-card>
              </div>
              <div class="col-sm-4">
                <v-card :width="cardWidthBreakPoint" :height="cardBreakPoint" class="pt-6 mx-auto">
                  <v-card-text class="text--h7">
                    COVID-19対策のため、<br>
                    ご予約可能時間を<br>
                    (月)(火)(金)(土)の10:00～15:00(施術開始時間)とさせていただきます。<br>
                    なお、ご連絡は前日19：00までにお願いします。<br>
                    ※ご予約は１日１名様限定となっております。
                  </v-card-text>
                  <v-card-text class="text--h7">
                    ※ご予約はお電話もしくは<br>
                    メールでお問い合わせください。
                  </v-card-text>
                </v-card>
              </div>
              <div class="col-sm-4 col-xs-12">
                <v-card :width="cardWidthBreakPoint" :height="cardBreakPoint"
                  class="d-flex justify-content-center align-items-center mx-auto">
                  <div id="map-box" class="w-75 h-75"></div>
                </v-card>
              </div>
            </div>
          </div>
        </v-bottom-navigation>
        
        <v-footer height="60" dark class="p-0 text-h4">
          <small class="m-auto" id="footer-letters">©2020 kassa-yuu</small>
        </v-footer>

  </div>
</template>