【手寫字體，古詩展示】

每次 Demo 只展示一位學生，不限制學生人數。

請把以下檔案放在同一資料夾：
index.html
student-font.ttf       ← 該學生的字型（可改成實際檔名，但需同步修改 index.html 的 demoConfig）
handwriting.txt        ← 該學生的手寫內容基準
background.mp3         ← Demo 背景音樂

修改學生姓名：
打開 index.html，找到 demoConfig：
studentName: "展示者姓名"
改成學生實際姓名即可。

TXT：
系統會忽略空白與換行，依 TXT 字元順序與詩句比對；比對成功的字標成紅色「手寫內容」，其餘標成藍色「機器生成」。

建議啟動方式（避免瀏覽器阻擋讀取 TXT/字型）：
在專案資料夾執行：
python -m http.server 8000
再開啟：
http://localhost:8000/
