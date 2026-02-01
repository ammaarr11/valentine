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
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    transition: all 0.3s ease;
  }

  .btn-yes {
    background: linear-gradient(45deg, #ff4d6d, #ff1a4d);
  }

  .btn-no {
    background: linear-gradient(45deg, #33cc33, #009900);
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
  <button id="yes" class="btn btn-yes">Yes</button>
  <button id="no" class="btn btn-no">No</button>
  <button id="areYouSure" class="btn btn-no hidden">Are you sure</button>
  <button id="reallySure" class="btn btn-no hidden">Are you really sure</button>
  <button id="reallyExtra" class="btn btn-no hidden">Really</button>
</div>

<script>
  const yesBtn = document.getElementById('yes');
  const noBtn = document.getElementById('no');
  const areYouSureBtn = document.getElementById('areYouSure');
  const reallySureBtn = document.getElementById('reallySure');
  const reallyExtraBtn = document.getElementById('reallyExtra');

  // الضغط على Yes
  yesBtn.addEventListener('click', () => {
    yesBtn.style.transform = 'scale(1.2)'; // يكبر تدريجيًا
    alert('🐥🐥');
  });

  // الضغط على No
  noBtn.addEventListener('click', () => {
    noBtn.classList.add('hidden');
    areYouSureBtn.classList.remove('hidden');
    yesBtn.style.transform = 'scale(1.5)';
  });

  // الضغط على Are you sure
  areYouSureBtn.addEventListener('click', () => {
    areYouSureBtn.classList.add('hidden');
    reallySureBtn.classList.remove('hidden');
    yesBtn.style.transform = 'scale(2)';
  });

  // الضغط على Are you really sure
  reallySureBtn.addEventListener('click', () => {
    reallySureBtn.classList.add('hidden');
    reallyExtraBtn.classList.remove('hidden');
    yesBtn.style.transform = 'scale(2.5)';
  });

  // الضغط على Really
  reallyExtraBtn.addEventListener('click', () => {
    reallyExtraBtn.classList.add('hidden');
    yesBtn.style.transform = 'scale(3)';
  });
</script>

</body>
</html>
