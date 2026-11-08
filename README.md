# to.flora
to.flora_from.emily
<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>To. Flora</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Nanum+Myeongjo:wght@400;700&family=Cormorant+Garamond:ital,wght@1,400&display=swap" rel="stylesheet">
<style>
:root{
  --walnut:#1a120e;
  --wood:#2c1e17;
  --parchment:#ece3d6;
  --dust:#b3a291;
  --wine:#8a2a3b;
  --wine-deep:#5c1623;
  --serif:'Nanum Myeongjo','Batang','Noto Serif KR',serif;
  --script:'Cormorant Garamond',Georgia,serif;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--walnut);color:var(--parchment);font-family:var(--serif);line-height:2.1;-webkit-font-smoothing:antialiased}
body.locked{overflow:hidden;height:100vh}

#cover{position:fixed;inset:0;z-index:10;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:2.5rem;text-align:center;
  background:linear-gradient(rgba(26,18,14,.55),rgba(26,18,14,.82)),url(images/envelope.jpg) center/cover no-repeat;
  transition:opacity 1.6s ease,visibility 0s linear 1.6s}
#cover.gone{opacity:0;visibility:hidden;pointer-events:none}
#cover h1{font-family:var(--script);font-style:italic;font-weight:400;font-size:clamp(3rem,11vw,6.5rem);letter-spacing:.02em;line-height:1.1;color:var(--parchment);text-shadow:0 2px 30px rgba(0,0,0,.6)}
.seal{position:relative;width:104px;height:104px;border:0;border-radius:52% 48% 55% 45%/48% 54% 46% 52%;cursor:pointer;color:#f1d9d9;font-family:var(--serif);font-size:.95rem;letter-spacing:.08em;
  background:radial-gradient(circle at 35% 30%,#b04558,var(--wine) 45%,var(--wine-deep));
  box-shadow:inset 0 0 0 5px rgba(0,0,0,.14),inset 0 3px 8px rgba(255,255,255,.18),0 10px 28px rgba(0,0,0,.55);
  transition:transform .5s ease,box-shadow .5s ease}
.seal::before{content:"";position:absolute;inset:12px;border:1px solid rgba(241,217,217,.35);border-radius:inherit}
.seal:hover{transform:scale(1.07) rotate(-3deg)}
.seal:focus-visible{outline:2px solid var(--parchment);outline-offset:6px}
.seal.pressed{transform:scale(.92);box-shadow:inset 0 0 0 5px rgba(0,0,0,.2),0 4px 12px rgba(0,0,0,.5)}

#letter{opacity:0;transition:opacity 2s ease .4s}
#letter.show{opacity:1}
section{display:flex;flex-direction:column;align-items:center;justify-content:center;padding:18vh 1.6rem}
.text{max-width:30rem;width:100%;text-align:left;font-size:clamp(1.02rem,2.6vw,1.2rem)}
.text p+p{margin-top:2.1em}
.text .l{display:block}

.opening{min-height:100vh;background:linear-gradient(var(--walnut),var(--wood))}

figure{width:min(100%,46rem);margin:0 auto;padding:0 1.2rem}
figure img{display:block;width:100%;height:auto;box-shadow:0 30px 70px rgba(0,0,0,.6)}
.photo{padding:6vh 0}
.photo.warm{background:var(--wood)}

.memory{background:linear-gradient(var(--wood),var(--walnut))}
.memory-2{background:var(--walnut)}

.fade-text{color:var(--dust)}
.wound{color:#e8c6c6;font-weight:700;text-shadow:0 0 22px rgba(138,42,59,.8);padding-left:1.1rem;border-left:2px solid var(--wine)}

.ending{min-height:100vh;background:linear-gradient(var(--walnut),#0f0a08)}
.from{margin-top:5rem;font-family:var(--script);font-style:italic;font-size:1.9rem;color:var(--dust);text-align:center}
.from::before{content:"";display:block;width:10px;height:10px;margin:0 auto 1.6rem;border-radius:50%;background:var(--wine);box-shadow:0 0 18px var(--wine)}

.rise{opacity:0;transform:translateY(14px);transition:opacity 1.4s ease,transform 1.4s ease}
.rise.in{opacity:1;transform:none}

@media (prefers-reduced-motion:reduce){
  html{scroll-behavior:auto}
  *{transition-duration:.01s!important}
  .rise{opacity:1;transform:none}
}
</style>
</head>
<body class="locked">

<div id="cover">
  <h1>To. Flora</h1>
  <button class="seal" id="open" aria-label="편지 열어보기">열어보기</button>
</div>

<main id="letter">

  <section class="opening">
    <div class="text rise">
      <p><span class="l">플로라, 잘 지냈어?</span>
        <span class="l">우리가 처음 만났을 때가 엊그제 같은데,</span>
        <span class="l">벌써 이렇게 커버렸네.</span></p>
    </div>
  </section>

  <div class="photo warm">
    <figure class="rise"><img src="images/sunflower.jpg" alt="해바라기밭 앞에서 손을 잡고 걷는 두 소녀" loading="lazy"></figure>
  </div>

  <section class="memory">
    <div class="text">
      <p class="rise"><span class="l">우리가 12년 전에 처음 만났잖아?</span>
        <span class="l">그때 처음 고아원에 와서 혼자였던 내게 먼저 손을 내밀어준 건</span>
        <span class="l">바로 너였어.</span></p>
      <p class="rise"><span class="l">네가 없었다면 지금의 나는 이 세상에 없었을 지도 몰라.</span>
        <span class="l">창백했던 내 얼굴에 홍조를 띄워준 것도,</span>
        <span class="l">닫혔던 내 입을 처음으로 열어 준 것도,</span>
        <span class="l">얼음장 같던 나를 따뜻하게 녹여 준 것도,</span>
        <span class="l">전부 너였어.</span></p>
      <p class="rise"><span class="l">나는 우리가 오래 갈 줄 알았지.</span>
        <span class="l">100년 뒤에도, 1000년 뒤에도 함께일 줄 알았어.</span></p>
    </div>
  </section>

  <div class="photo">
    <figure class="rise"><img src="images/fade.jpg" alt="색이 바래며 한 소녀가 지워진 해바라기밭의 장면" loading="lazy"></figure>
  </div>

  <section class="memory-2">
    <div class="text">
      <p class="rise fade-text"><span class="l">근데, 세상 일이 내 상상대로 흘러가지 않더라.</span>
        <span class="l">너도 나처럼 좋은 집에 입양되어 행복하게 살 줄 알았어.</span>
        <span class="l">그 쓰레기 같은 새끼들한테 네가 넘어가지만 않았으면,</span>
        <span class="l">넌 지금쯤 내 옆에서 환하게 웃고 있었을 텐데.</span></p>
    </div>
  </section>

  <div class="photo warm">
    <figure class="rise"><img src="images/memorial.jpg" alt="흰 국화와 촛불에 둘러싸인 영정사진" loading="lazy"></figure>
  </div>

  <section class="ending">
    <div class="text">
      <p class="rise wound">원장이라는 놈이 그 새끼들한테 너를 팔지만 않았어도...</p>
      <p class="rise"><span class="l">네 마지막 가는 길은 내가 배웅해 주고파.</span>
        <span class="l">언제까지나, 볼 수 없는 형태로 존재하더라도...</span>
        <span class="l">영원토록 내 곁에 있어줄 거지?</span></p>
      <p class="rise"><span class="l">기다릴게. 천천히 와도 돼.</span></p>
      <p class="from rise">From. Emily</p>
    </div>
  </section>

</main>

<script>
(function(){
  var body=document.body, cover=document.getElementById('cover'),
      letter=document.getElementById('letter'), btn=document.getElementById('open');

  btn.addEventListener('click',function(){
    btn.classList.add('pressed');
    setTimeout(function(){
      cover.classList.add('gone');
      letter.classList.add('show');
      body.classList.remove('locked');
      window.scrollTo(0,0);
    },350);
  });

  var els=document.querySelectorAll('.rise');
  if('IntersectionObserver' in window){
    var io=new IntersectionObserver(function(entries){
      entries.forEach(function(e){
        if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target);}
      });
    },{threshold:.25});
    els.forEach(function(el){io.observe(el)});
  }else{
    els.forEach(function(el){el.classList.add('in')});
  }
})();
</script>
</body>
</html>
