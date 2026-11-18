# Bar-REST
<!doctype html>
<html lang="ja">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>BAR REST MENU</title>
  <style>
    :root {
      color-scheme: dark;
      --bg: #111111;
      --surface: #191919;
      --text: #f5f5f3;
      --muted: #b8b8b5;
      --line: #383836;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: var(--bg);
      color: var(--text);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans JP", sans-serif;
      font-size: 16px;
      line-height: 1.6;
    }

    .page {
      width: min(100% - 40px, 900px);
      margin: 0 auto;
      padding: 54px 0 64px;
    }

    header {
      padding: 0 0 28px;
      border-bottom: 1px solid var(--line);
      text-align: center;
    }

    h1 {
      margin: 0;
      font-size: clamp(2.25rem, 7vw, 3.5rem);
      font-weight: 600;
      letter-spacing: .14em;
      line-height: 1.15;
    }

    h1 span {
      display: block;
    }

    h1 .menu-word {
      margin-top: 8px;
      font-size: .43em;
      font-weight: 400;
      letter-spacing: .32em;
    }

    .intro {
      max-width: 680px;
      margin: 22px auto 0;
      color: var(--muted);
      text-align: center;
    }

    .guide {
      max-width: 680px;
      margin: 26px auto 38px;
      padding: 18px 22px;
      border: 1px solid var(--line);
      background: var(--surface);
    }

    h2 {
      margin: 0 0 12px;
      font-size: 1rem;
      font-weight: 600;
      letter-spacing: .06em;
    }

    .guide p {
      margin: 5px 0;
      color: var(--muted);
    }

    .menu-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 16px;
    }

    .category {
      min-width: 0;
      padding: 18px 20px 19px;
      border: 1px solid var(--line);
      background: var(--surface);
    }

    .category h2 {
      padding-bottom: 10px;
      border-bottom: 1px solid var(--line);
    }

    .category p {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      gap: 12px;
      margin: 7px 0 0;
      color: var(--muted);
      overflow-wrap: anywhere;
    }

    .category p span:first-child {
      min-width: 0;
    }

    .category p span:last-child {
      flex: 0 0 auto;
      color: var(--text);
    }

    .happy-hour {
      margin-top: 22px;
      padding: 20px 22px;
      border: 1px solid var(--line);
      background: var(--surface);
    }

    .happy-hour p {
      margin: 6px 0 0;
      color: var(--muted);
    }

    footer {
      margin-top: 22px;
      padding: 18px 22px;
      border-top: 1px solid var(--line);
      color: var(--muted);
    }

    footer p {
      margin: 5px 0;
    }

    @media (max-width: 640px) {
      .page {
        width: min(100% - 32px, 520px);
        padding: 36px 0 48px;
      }

      .menu-grid {
        grid-template-columns: 1fr;
        gap: 12px;
      }

      .guide,
      .category,
      .happy-hour {
        padding-left: 16px;
        padding-right: 16px;
      }
    }
  </style>
</head>
<body>
  <main class="page">
    <header>
      <h1>
        <span>BAR REST</span>
        <span class="menu-word">MENU</span>
      </h1>
      <p class="intro">ご注文がお決まりになりましたら、スタッフまでお声がけください。</p>
    </header>

    <section class="guide" aria-labelledby="guide-title">
      <h2 id="guide-title">ご利用案内</h2>
      <p>・他のお客様のご迷惑になる行為は、ご遠慮ください。</p>
      <p>・スタッフの案内に従っていただけない場合は、ご退店して頂く場合がございます。</p>
    </section>

    <section class="menu-grid" aria-label="メニュー">
      <article class="category">
        <h2>ビール</h2>
        <p><span>・サントリー生ビール</span><span>₩ 7,000</span></p>
        <p><span>・ビールカクテル（レッドアイ・シャンディガフ）</span><span>₩8,000</span></p>
      </article>

      <article class="category">
        <h2>サワー（レモン・ピーチ・マスカット・梅・カルピス）</h2>
        <p><span>・各種</span><span>₩ 6,000</span></p>
      </article>

      <article class="category">
        <h2>ハウスウィスキー（KENTUCKY GENTLEMEN)</h2>
        <p><span>・ハイボール</span><span>₩5,000</span></p>
        <p><span>・その他</span><span>₩6,000</span></p>
      </article>

      <article class="category">
        <h2>その他ウィスキー</h2>
        <p><span>・各種</span><span>₩9,000</span></p>
      </article>

      <article class="category">
        <h2>カクテル（ピーチ・カシス・ウォッカ・ジン・カルーア・マリブ）</h2>
        <p><span>・各種</span><span>₩ 7,000</span></p>
      </article>

      <article class="category">
        <h2>焼酎（참이술・いいちこ・黒霧・茉莉花・DAIAME)</h2>
        <p><span>・참이술系</span><span>₩ 6,000</span></p>
        <p><span>・その他</span><span>₩ 8,000</span></p>
      </article>

      <article class="category">
        <h2>ノンアルコール</h2>
        <p><span>・各種</span><span>₩ 6,000</span></p>
      </article>

      <article class="category">
        <h2>ショット</h2>
        <p><span>・各種</span><span>₩7,000</span></p>
        <p><span>・観覧車</span><span>₩130,000（1800アネホは別料金）</span></p>
        <p><span>・1800アネホ</span><span>₩15,000</span></p>
      </article>

      <article class="category">
        <h2>ボトル</h2>
        <p><span>・各種</span><span>₩ 250,000</span></p>
        <p><span>・その他 ask</span></p>
      </article>

      <article class="category">
        <h2>シャンパン</h2>
        <p><span>・ブランプシー</span><span>₩150,000</span></p>
        <p><span>・オリシャン</span><span>₩200,000</span></p>
        <p><span>・ヴーヴイエロー</span><span>₩250,000</span></p>
        <p><span>・モエロゼ</span><span>₩350,000</span></p>
        <p><span>・ベルエポ</span><span>₩65,000</span></p>
        <p><span>・その他 ask</span></p>
      </article>

      <article class="category">
        <h2>乾き物•안주</h2>
        <p><span>・</span><span>₩ 5,000</span></p>
      </article>
    </section>

    <section class="happy-hour">
      <h2>Happy Hour （3時〜5時）</h2>
      <p>飲み放題1人₩35,000</p>
      <p>※ビール・ショット・ボトル・シャンパンは別料金です。</p>
    </section>

    <footer>
      <p>フード持ち込みチャージ　1卓₩8,000</p>
      <p>ボトルキープチャージ　1人₩10,000</p>
    </footer>
  </main>
</body>
</html>