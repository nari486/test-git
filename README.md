<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>과외방·사고팔고방·커뮤니티방</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');
    body {
      font-family: 'Montserrat', sans-serif;
      background-color: #fbeff3; /* 파스텔 와인색 배경 */
      color: #3d1f2b;
      margin: 0;
      padding: 0;
    }
    header {
      background: linear-gradient(90deg, #d7a7b3 0%, #e8b6c1 100%);
      color: #3d1f2b;
      padding: 24px 0 18px 0;
      text-align: center;
      font-size: 2.2em;
      font-weight: 700;
      letter-spacing: 2px;
      box-shadow: 0 4px 8px rgba(200, 120, 150, 0.08);
    }
    nav {
      background: #f6dbe4;
      display: flex;
      justify-content: center;
      gap: 40px;
      padding: 15px 0;
      box-shadow: 0 2px 6px rgba(200, 120, 150, 0.06);
    }
    nav a {
      color: #a05c7b;
      text-decoration: none;
      font-weight: 600;
      font-size: 1.1em;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: #d48ca6;
    }
    main {
      max-width: 900px;
      margin: 30px auto;
      background: #fff8fb;
      border-radius: 14px;
      padding: 32px;
      color: #3d1f2b;
      box-shadow: 0 4px 12px rgba(200, 120, 150, 0.10);
    }
    section {
      margin-bottom: 40px;
    }
    h2 {
      color: #a05c7b;
      border-bottom: 2px solid #e8b6c1;
      padding-bottom: 8px;
      margin-bottom: 20px;
      font-weight: 700;
      font-size: 1.3em;
      display: flex;
      align-items: center;
      gap: 8px;
    }
    .card-list {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }
    .card {
      background: #f6dbe4;
      border: 1px solid #e8b6c1;
      border-radius: 10px;
      padding: 18px;
      width: 250px;
      box-sizing: border-box;
      box-shadow: 0 2px 6px rgba(200, 120, 150, 0.08);
      transition: transform 0.3s ease;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 6px 12px rgba(200, 120, 150, 0.18);
    }
    .card strong {
      color: #a05c7b;
      display: block;
      margin-bottom: 8px;
      font-weight: 700;
    }
    .card button {
      background: #a05c7b;
      color: white;
      border: none;
      border-radius: 6px;
      padding: 8px 16px;
      margin-top: 12px;
      cursor: pointer;
      font-weight: 600;
      transition: background 0.3s ease;
    }
    .card button:hover {
      background: #d48ca6;
    }
    .post {
      background: #f6dbe4;
      border-radius: 8px;
      padding: 16px;
      margin-bottom: 18px;
      border-left: 4px solid #e8b6c1;
    }
    .post strong {
      color: #a05c7b;
    }
    form {
      margin-top: 10px;
    }
    input, button {
      padding: 8px 12px;
      margin: 6px 0;
      border-radius: 6px;
      border: 1px solid #e8b6c1;
      font-size: 1em;
      font-family: 'Montserrat', sans-serif;
    }
    button[type="submit"] {
      background: #a05c7b;
      color: white;
      border: none;
      font-weight: 700;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    button[type="submit"]:hover {
      background: #d48ca6;
    }
    @media (max-width: 700px) {
      .card-list { flex-direction: column; gap: 12px; }
      main { padding: 14px; }
    }
  </style>
</head>
<body>
  <header>과외방 · 사고팔고방 · 커뮤니티방</header>
  <nav>
    <a href="#tutor">📚 과외방</a>
    <a href="#market">💸 사고팔고방</a>
    <a href="#community">🗨️ 커뮤니티방</a>
  </nav>
  <main>
    <section id="tutor">
      <h2>📚 과외방</h2>
      <div class="card-list">
        <div class="card">
          <strong>김수학</strong>
          <p>과목: 수학</p>
          <p>경력: 5년</p>
          <button>문의하기</button>
        </div>
        <div class="card">
          <strong>이영어</strong>
          <p>과목: 영어</p>
          <p>경력: 3년</p>
          <button>문의하기</button>
        </div>
      </div>
    </section>
    <section id="market">
      <h2>💸 사고팔고방</h2>
      <div class="card-list">
        <div class="card">
          <strong>중고 노트북</strong>
          <p>가격: 300,000원</p>
          <p>상태: 양호</p>
          <button>구매문의</button>
        </div>
        <div class="card">
          <strong>수학 참고서</strong>
          <p>가격: 8,000원</p>
          <p>상태: 깨끗함</p>
          <button>구매문의</button>
        </div>
      </div>
    </section>
    <section id="community">
      <h2>🗨️ 커뮤니티방</h2>
      <div class="post">
        <strong>공부 팁 공유해요!</strong> (by 홍길동)
        <p>효율적으로 암기하는 방법 추천해 주세요!</p>
      </div>
      <div class="post">
        <strong>중고거래 후기</strong> (by 이몽룡)
        <p>좋은 거래 감사합니다 :)</p>
      </div>
      <form>
        <input type="text" placeholder="제목" required>
        <input type="text" placeholder="작성자" required>
        <br>
        <input type="text" placeholder="내용" style="width:70%;" required>
        <button type="submit">글쓰기</button>
      </form>
    </section>
  </main>
</body>
</html>
