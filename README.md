<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Simple Progress Bar</title>
  <link rel="stylesheet" media="all" href="style.css" />
 <style>
  body {
  justify-content: center;
  align-items: center;
  background: #000;
  display: flex;
  height: 100vh;
  padding: 0;
  margin: 0;
}

.progress {
  background: rgba(255,255,255,0.1);
  justify-content: flex-start;
  border-radius: 100px;
  align-items: center;
  position: relative;
  padding: 0 5px;
  display: flex;
  height: 40px;
  width: 500px;
}

.progress-value {
  animation: load 3s normal forwards;
  box-shadow: 0 10px 40px -10px #fff;
  border-radius: 100px;
  background: #fff;
  height: 30px;
  width: 0;
}

@keyframes load {
  0% { width: 0; }
  100% { width: 68%; }
}
 </style>
</head>
<body>
<div class="progress">
  <div class="progress-value"></div>
</div>
</body>
