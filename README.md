<html>
<head>
	<title>봉사활동프로젝트</title>
    	<style>
        body {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            margin: 0 auto;
            height: 125vh;
            background-color: #f1f1f1;
        }
        form {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        label, select, input, button {
            margin-bottom: 10px;
        }
    </style>
    <script>
        let timerInterval;
        let elapsedTime = 0;

        function startTimer() {
            clearInterval(timerInterval);
            elapsedTime = 0;
            document.getElementById('timer').textContent = `경과 시간: ${elapsedTime} 초`;

            timerInterval = setInterval(() => {
                elapsedTime += 1;
                document.getElementById('timer').textContent = `경과 시간: ${elapsedTime} 초`;
            }, 1000);
        }

        function stopTimer() {
            clearInterval(timerInterval);
        }

        function handleSubmit(event) {
            event.preventDefault();
            const selectedOption1 = document.getElementById('sub1').value;
            const selectedOption2 = document.getElementById('sub2').value;
	const selectedOption3 = document.getElementById('sub3').value;


            document.getElementById('result').textContent = `내가 선택한 과목: ${selectedOption1}, ${selectedOption2},${selectedOption3}`;
        }
    </script>
</head>
<body>
    <form onsubmit="handleSubmit(event)">
        <label for="sub1">과목 선택 1</label>
        <select name="subject1" id="sub1">
            <option value="영어">영어</option>
            <option value="국어">국어</option>
            <option value="수학">수학</option>
            <option value="한국사">한국사</option>
            <option value="탐구1">탐구1</option>
            <option value="탐구2">탐구2</option>
        </select>

        <label for="sub2">과목 선택 2</label>
        <select name="subject2" id="sub2">
            <option value="영어">영어</option>
            <option value="국어">국어</option>
            <option value="수학">수학</option>
            <option value="한국사">한국사</option>
            <option value="탐구1">탐구1</option>
            <option value="탐구2">탐구2</option>
        </select>

<label for="sub2">과목 선택 3</label>
        <select name="subject3" id="sub3">
            <option value="영어">영어</option>
            <option value="국어">국어</option>
            <option value="수학">수학</option>
            <option value="한국사">한국사</option>
            <option value="탐구1">탐구1</option>
            <option value="탐구2">탐구2</option>
        </select>

        <input type="submit" value="제출" />
    </form>

    <p >_____________________</p>
    <button onclick="startTimer()">타이머 시작</button>
    <p id="timer">경과 시간: 0 초</p>
    <button onclick="stopTimer()">타이머 멈춤</button>
    
    <p id="result"></p>
<p >_____________________</p>
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-sg5v{border-color:inherit;font-size:100%;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg"><thead>
  <tr>
    <th class="tg-0pky"></th>
    <th class="tg-0pky">월</th>
    <th class="tg-0pky">화</th>
    <th class="tg-0pky">수</th>
    <th class="tg-0pky">목</th>
    <th class="tg-sg5v">금</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0pky">1교시</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">2교시</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">3교시</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">4교시</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">5교시</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">6교시</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">7교시</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
</tbody></table>
<p >_____________________</p>
</body>
</html>

