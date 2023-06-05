# Welcome to our website.

## Hello. My name is Seung-gu Jeong, a student at Semyeong University.  I am studying with the goal of becoming a backend developer.


<!DOCTYPE html>
<html>
<head>
  <title>HTML 예시</title>
  <style>
    .content {
      display: none;
      margin-top: 10px;
    }
    
    .content.show {
      display: block;
    }
  </style>
  <script>
    function showTab(tabName) {
      var tabs = document.getElementsByClassName('content');
      for (var i = 0; i < tabs.length; i++) {
        tabs[i].classList.remove('show');
      }
  
      document.getElementById(tabName).classList.add('show');
    }
  </script>
</head>
<body>
  <header>
    <h1>Let me introduce myself.</h1>
    <nav>
      <ul>
        <li><a href="#" onclick="showTab('learned')">Things I have learned</a></li>
        <li><a href="#" onclick="showTab('learning')">Things I am learning</a></li>
        <li><a href="#" onclick="showTab('want')">Things I want to learn</a></li>
      </ul>
    </nav>
  </header>
  
  <main>
    <h2>콘텐츠 제목</h2>
    <p>이곳에 내용을 작성합니다.</p>
    <img src="이미지 주소" alt="이미지 설명">
    
    <div id="learned" class="content">
        <img src="https://img.shields.io/badge/C++-Language-blue?style=social" alt="C++ Language Badge">
    </div>
  
    <div id="learning" class="content">
      <!-- 배우고 있는 프로그래밍 언어 뱃지들을 여기에 추가하세요 -->
    </div>
  
    <div id="want" class="content">
      <!-- 배우고 싶은 프로그래밍 언어 뱃지들을 여기에 추가하세요 -->
    </div>
  </main>
  
  <footer>
    <p>Email: songkoo0229@gmail.com</p>
  </footer>
</body>
</html>