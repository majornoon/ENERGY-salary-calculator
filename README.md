<!DOCTYPE html>
<html lang="en">
<head>
  <meta name="google-site-verification" content="AIa4brVmDEemQMxzaZnn_NK--GqzPsNniOFmoCnMhNc" />
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Salary Calculator</title>
  <style>
    input[type="number"], input[type="text"] {    
      width: 100%;
      padding: 8px; 
      margin-top: 5px;
      opacity: 0.85;
      background-color: rgba(255, 255, 255, 0.2);
      color: #fff;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    body {
      font-family: Arial, sans-serif;
      background-image: url('https://lh3.googleusercontent.com/a/ACg8ocLX5f5tpjfubtA97Wdsue10X6kvPnRpG1SjTv7_lL3B7gbPvVsc=s288-c-no');
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center center;
      color: #fff;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }
    .container {
      max-width: 600px;
      margin: 50px auto;
      background-color: rgba(0, 0, 0, 0.7);
      padding: 20px;
      border-radius: 10px;
    }
    h2 {
      text-align: center;
    }
    label {
      display: block;
      margin-top: 15px;
    }
    button {
      margin-top: 20px;
      padding: 10px;
      width: 100%;
      background-color: #28a745;
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .result {
      margin-top: 20px;
      font-size: 18px;
    }
    footer {
      text-align: center;
      padding: 15px;
      margin-top: auto;
      background-color: rgba(0, 0, 0, 0.6);
      color: #ccc;
      font-size: 14px;
    }
  </style>
</head>
<body>
<div class="container">
  <h2>Salary Calculator</h2>
  <label>Name:
    <input type="text" id="userName" placeholder="James-monis">
  </label>
  <label>Basic Salary Onshore:
    <input type="number" id="basicOnshore" placeholder="e.g., 1400">
  </label>
  <label>Basic Salary Offshore:
    <input type="number" id="basicOffshore" placeholder="e.g., 1500">
  </label>
  <label>Days Worked Onshore:
    <input type="number" id="onshoreDays" value="0">
  </label>
  <label>Days Worked Offshore:
    <input type="number" id="offshoreDays" value="0">
  </label>
  <label>Idle Days:
    <input type="number" id="idleDays" value="0">
  </label>
  <label>Normal Overtime Hours (Onshore):
    <input type="number" id="normalOtOnshore" value="0">
  </label>
  <label>Normal Overtime Hours (Offshore):
    <input type="number" id="normalOtOffshore" value="0">
  </label>
  <label>Friday Overtime Days (Onshore):
    <input type="number" id="fridayOtOnshore" value="0">
  </label>
  <label>Friday Overtime Days (Offshore):
    <input type="number" id="fridayOtOffshore" value="0">
  </label>
  <label>Absent Days:
    <input type="number" id="absentDays" value="0">
  </label>

  <button onclick="calculateSalary()">Calculate Salary</button>

  <div class="result" id="result"></div>
</div>

<footer>

