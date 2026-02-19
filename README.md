
<!DOCTYPE html>
<html>
<head>
<title>QA Automation Assistant</title>
<link rel='stylesheet' href='assets/styles.css'>
<script src='https://cdn.jsdelivr.net/npm/xlsx@0.18.5/dist/xlsx.full.min.js'></script>
<script src='assets/app.js'></script>
</head>
<body>
<img src='assets/logo.png' style='height:50px;'>
<h2>QA Automation Assistant</h2>
<div class='progress'><div id='progress-bar' class='progress-bar'></div></div>
<div class='step'>
<h3>Step 1</h3>
<input id='datepicker' type='date'><br><br>
<input id='folderInput' type='file' webkitdirectory directory multiple><br>
<input id='destInput' type='file' webkitdirectory directory multiple><br><br>
<button onclick='step1()'>Copy Folder</button>
<p id='step1-status'></p>
</div>
<div class='step'>
<h3>Step 2</h3>
<input id='excelInput' type='file' accept='.xlsx,.xls'><br>
<button id='btn-step2' class='disabled' onclick='step2()'>Process Excel</button>
<p id='step2-status'></p>
</div>
<div class='step'>
<h3>Step 3</h3>
<input id='fileA' type='file'><br>
<input id='fileB' type='file'><br>
<button id='btn-step3' class='disabled' onclick='step3()'>Calculate Delta</button>
<p id='step3-status'></p>
</div>
<div class='step'>
<h3>Step 4</h3>
<button id='btn-step4' class='disabled' onclick='step4()'>Generate Report</button>
<p id='step4-status'></p>
</div>
<div class='step'>
<h3>Step 5</h3>
<button id='btn-post1' class='disabled' onclick="postToTeams('Area1')">Post to Area 1</button>
<button id='btn-post2' class='disabled' onclick="postToTeams('Area2')">Post to Area 2</button>
<p id='teams-status'></p>
</div>
</body>
</html>
