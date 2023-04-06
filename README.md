<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>

  <style>
    body {
      font-size: 1.24em;
    }
    div {
      padding: 24px;
      box-sizing: border-box;
      background-color: pink;
      width: 24em;
    }
    p {
      width: 24em;
    }
    span {
      background-color: skyblue;
    }
  </style>

  <style>
    div {
      position: relative;
      width: 160px;
     height: 160px;
      border: 2px solid rgba(255, 255, 255, 0.33);
    }
    .red {
      background-color: tomato;
    }
    .blue {
     background-color: dodgerblue;
      top: 96px;
      left: 96px;
    }
    .yellow {
      background-color: yellow;
     border: 2px solid gold;
     width: inherit;
     height: inherit;
     padding: 24px;
     top: 160px;
     left: 160px;
   }
  </style>

  <style>
    .result > div {
      display: inline-block;
      width: 160px;
     height: 160px;
     line-height: 160px;
     text-align: center;
     font-weight: bold;
     font-size: 1.2em;
     color: white;
     background-color: blueviolet;
     cursor: pointer;
   }
    .result > div.red { background-color: tomato; }
    .result > div.green { background-color: olivedrab; }
    .result > div.blue { background-color: dodgerblue; }
  </style>

  <title>Inline vs Block</title>

</head>

<!-- textshadow-->
<body>
  <main>
    <section class="result">

      <!-- 시작 -->

      <p>
        안녕하세요, 저는 컴퓨터공학과 21학번 김연수입니다.
      </p>

      <!-- 끝 -->

    </section>
    <section class="controls"></section>
  </main>

  <script>
    const controls = [
      {
        obj: {
          name: 'p 요소',
          query: 'p'
        },
        fields: [
          {
            type: 'select',
            style: 'text-shadow',
            opts: [
              'none',
              '2px 2px lightgrey',
              '3px -3px 4px blue',
              '0 1px red, 0 -1px red, 1px 0 red, -1px 0 red'
            ]
          },
        ]
      },
    ]
  </script>
</body>
<!-- block&inline-->
<body>

  <div>
    <strong>나의 관심사</strong>
  </div>

  <br>

  <p>
    요즘 저의 관심사는 <span>맛집 방문</span> 입니다.
  </p>
  <p>거창하지는 않지만, 일상 속에서 행복을 발견할 수 있는 가장 접근성 높은 취미라고 생각합니다.</p>
  
</body>
<!--포지셔닝-->
<body>

  <main>
    <section class="result">

      <!-- 시작 -->

      <div class="skyblue">
        <img src="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2FMjAxOTAzMTVfMjgg%2FMDAxNTUyNjIzNTI3ODcz.min-WJr6_YxYcli0CpCf_eHEVv_FykNKeuQs7n6ZOtgg.JUhb9-ZQkONLhIaJHr6EI-uXWKC1ZaIHuPhLvWEWmnUg.JPEG.wac11229%2FScreenshot_20190314-214938_Naver_Blog.jpg&type=sc960_832" alt=""></p>  
    
      </div>

      <!-- 끝 -->

    </section>
    <section class="controls"></section>
  </main>  
  
</body>


<!--hidden-->
<body>
  <main>
    <section class="result">

      <!-- 시작 -->

      <div class="green">클릭!</div>

      <p>
        <strong>visibility</strong> 속성을 <em>hidden</em>으로 하면 위 효과에 더하여 <br>
        마우스 오버 효과나 포커스, 클릭 등도 무효하게 됩니다. <br>
        스크린 리더에게도 읽히지 않게 되죠.
      </p>
 

      <!-- 끝 -->

    </section>
    <section class="controls"></section>
  </main>

  <script>
    const controls = [
      
      {
        obj: {
          name: '초록색 div',
          query: '.green'
        },
        fields: [
          {
            type: 'radio',
            style: 'visibility',
            opts: [
              'visible',
              'hidden'
            ]
          },
        ]
      }
    ]
  </script>
  
</body>
<!--viewport-->

</html>
