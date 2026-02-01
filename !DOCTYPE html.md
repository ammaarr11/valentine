<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Valentine</title>  
<style>  
  body {  
    margin: 0;  
    font-family: Arial, sans-serif;  
    text-align: center;  
    background: url('https://i.ibb.co/3fB0rQz/owl-heart.jpg') no-repeat center center;  
    background-size: cover;  
    height: 100vh;  
    display: flex;  
    flex-direction: column;  
    justify-content: center;  
    align-items: center;  
  }  
  h1 {  
    color: #fff;  
    font-size: 2rem;  
    text-shadow: 2px 2px 5px #000;  
  }  
  .btn {  
    padding: 10px 30px;  
    margin: 10px;  
    font-size: 1.2rem;  
    border: none;  
    cursor: pointer;  
    border-radius: 10px;  
    color: white;  
    background-color: red;  
    transition: all 0.3s ease;  
  }  
  .hidden {  
    display: none;  
  }  
</style>  
</head>  
<body>  
  
<h1>Manal, will you be my valentine?</h1>  
<button id="yes" class="btn">Yes</button>  
<button id="no" class="btn">No</button>  
<button id="areYouSure" class="btn hidden">Are you sure</button>  
<button id="reallySure" class="btn hidden">Are you really sure</button>  
<button id="reallyExtra" class="btn hidden">Really</button>  
  
<script>  
  const yesBtn = document.getElementById('yes');  
  const noBtn = document.getElementById('no');  
  const areYouSureBtn = document.getElementById('areYouSure');  
  const reallySureBtn = document.getElementById('reallySure');  
  const reallyExtraBtn = document.getElementById('reallyExtra');  
  
  // اضغط على Yes  
  yesBtn.addEventListener('click', () => {  
    alert('🐥🐥');  
  });  
  
  // اضغط على No  
  noBtn.addEventListener('click', () => {  
    yesBtn.style.transform = 'scale(1.5)';  
    noBtn.style.transform = 'scale(0.7)';  
    noBtn.style.opacity = '0.5';  
    areYouSureBtn.classList.remove('hidden');  
  });  
  
  // اضغط على Are you sure  
  areYouSureBtn.addEventListener('click', () => {  
    yesBtn.style.transform = 'scale(2)';  
    areYouSureBtn.style.transform = 'scale(0.6)';  
    areYouSureBtn.innerText = 'Are you really sure';  
    reallySureBtn.classList.remove('hidden');  
  });  
  
  // اضغط على Are you really sure  
  reallySureBtn.addEventListener('click', () => {  
    yesBtn.style.transform = 'scale(2.5)';  
    reallySureBtn.style.transform = 'scale(0.5)';  
    reallyExtraBtn.classList.remove('hidden');  
  });  
  
  // اضغط على Really  
  reallyExtraBtn.addEventListener('click', () => {  
    yesBtn.style.transform = 'scale(3)';  
    reallyExtraBtn.style.transform = 'scale(0.5)';  
  });  
</script>  
  
</body>  
</html>  
