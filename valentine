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
    background: #ffe6f0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
  }

  .owl-img {
    width: 180px;
    margin-bottom: 20px;
  }

  h1 {
    font-size: 2.5rem;
    color: #d9004c;
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
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    transition: all 0.3s ease;
  }

  .btn:hover {
    transform: scale(1.1);
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
  }

  .btn-yes {
    background: linear-gradient(45deg, #ff4d6d, #ff1a4d);
  }

  .btn-no {
    background: linear-gradient(45deg, #33cc33, #009900);
  }

  .hidden {
    display: none;
  }
</style>
</head>
<body>

<img src="https://content.mycutegraphics.com/graphics/valentine/valentines-day-owl.png" class="owl-img" alt="Valentine Owl">

<h1>Manal, will you be my Valentine?</h1>

<div id="buttons">
  <button id="yes" class="btn btn-yes">Yes</button>
  <button id="no" class="btn btn-no">No</button>
  <button id="areYouSure" class="btn btn-no hidden">Are you sure?</button>
  <button id="reallySure" class="btn btn-no hidden">Are you really sure?</button>
  <button id="reallyExtra" class="btn btn-no hidden">Really?</button>
</div>

<script>
  const yesBtn = document.getElementById('yes');
  const noBtn = document.getElementById('no');
  const areYouSureBtn = document.getElementById('areYouSure');
  const reallySureBtn = document.getElementById('reallySure');
  const reallyExtraBtn = document.getElementById('reallyExtra');

  // عند الضغط على Yes
  yesBtn.addEventListener('click', () => {
    yesBtn.style.transform = 'scale(1.5)';
    alert('🐥🐥');
  });

  // عند الضغط على No
  noBtn.addEventListener('click', () => {
    noBtn.classList.add('hidden');        // نخفي No
    areYouSureBtn.classList.remove('hidden'); // نظهر Are you sure
    yesBtn.style.transform = 'scale(1.3)';   // نكبر Yes شوي
  });

  // عند الضغط على Are you sure?
  areYouSureBtn.addEventListener('click', () => {
    areYouSureBtn.classList.add('hidden');
    reallySureBtn.classList.remove('hidden');
    yesBtn.style.transform = 'scale(1.6)';
  });

  // عند الضغط على Are you really sure?
  reallySureBtn.addEventListener('click', () => {
    reallySureBtn.classList.add('hidden');
    reallyExtraBtn.classList.remove('hidden');
    yesBtn.style.transform = 'scale(1.9)';
  });

  // عند الضغط على Really?
  reallyExtraBtn.addEventListener('click', () => {
    reallyExtraBtn.classList.add('hidden');
    yesBtn.style.transform = 'scale(2.2)';
  });
</script>

</body>
</html>
