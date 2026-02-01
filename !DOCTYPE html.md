<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Valentine for Manal</title>  
<style>  
  body {  
    margin: 0;  
    font-family: 'Arial', sans-serif;  
    background: #ffe6f0; /* خلفية فاتحة لطيفة */  
    display: flex;  
    flex-direction: column;  
    justify-content: center;  
    align-items: center;  
    height: 100vh;  
    text-align: center;  
  }  
  
  /* صورة البومة فوق النص */  
  .owl-img {  
    width: 150px;  
    margin-bottom: 20px;  
  }  
  
  h1 {  
    font-size: 2.5rem;  
    color: #ff3366;  
    text-shadow: 2px 2px 8px #ffccd5;  
    margin-bottom: 30px;  
  }  
  
  .btn {  
    padding: 15px 40px;  
    margin: 10px;  
    font-size: 1.5rem;  
    border: none;  
    border-radius: 15px;  
    cursor: pointer;  
    color: white;  
    background: linear-gradient(45deg, #ff4d6d, #ff1a4d);  
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);  
    transition: all 0.3s ease;  
  }  
  
  .btn:hover {  
    transform: scale(1.1);  
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);  
  }  
  
  .hidden {  
    display: none;  
  }  
</style>  
</head>  
<body>  
  
<img src="https://i.ibb.co/3fB0rQz/owl-heart.jpg" alt="Owl with heart" class="owl-img">  
  
<h1>Manal, will you be my Valentine?</h1>  
  
<div id="buttons">  
  <button id="yes" class="btn">Yes</button>  
  <button id="no" class="btn">No</button>  
  <button id="areYouSure" class="btn hidden">Are you sure</button>  
  <button id="reallySure" class="btn hidden">Are you really sure</button>  
  <button id="reallyExtra" class="btn hidden">Really</button>  
</div>  
  
<script>  
  const yesBtn = document.getElementById('yes');  
  const noBtn = document.getElementById('no');  
  const areYouSureBtn = document.getElementById('areYouSure');  
  const reallySureBtn = document.getElementById('reallySure');  
  const reallyExtraBtn = document.getElementById('reallyExtra');  
  
  // الضغط على Yes  
  yesBtn.addEventListener('click', () => {  
    alert('🐥🐥');  
  });  
  
  // الضغط على No  
  noBtn.addEventListener('click', () => {  
    yesBtn.style.transform = 'scale(1.5)';  
    noBtn.style.transform = 'scale(0.7)';  
    noBtn.style.opacity = '0.5';  
    areYouSureBtn.classList.remove('hidden');  
  });  
  
  // الضغط على Are you sure  
  areYouSureBtn.addEventListener('click', () => {  
    yesBtn.style.transform = 'scale(2)';  
    areYouSureBtn.style.transform = 'scale(0.6)';  
    areYouSureBtn.innerText = 'Are you really sure';  
    reallySureBtn.classList.remove('hidden');  
  });  
  
  // الضغط على Are you really sure  
  reallySureBtn.addEventListener('click', () => {  
    yesBtn.style.transform = 'scale(2.5)';  
    reallySureBtn.style.transform = 'scale(0.5)';  
    reallyExtraBtn.classList.remove('hidden');  
  });  
  
  // الضغط على Really  
  reallyExtraBtn.addEventListener('click', () => {  
    yesBtn.style.transform = 'scale(3)';  
    reallyExtraBtn.style.transform = 'scale(0.5)';  
  });  
</script>  
  
</body>  
</html>  
