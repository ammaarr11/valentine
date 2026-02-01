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
    background: linear-gradient(120deg, #ffe6f0, #fff0e6);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
    overflow: hidden;
  }

  .owl-img {
    width: 180px;
    margin-bottom: 20px;
    animation: float 3s ease-in-out infinite;
  }

  @keyframes float {
    0%,100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
  }

  h1 {
    font-size: 2.5rem;
    color: #006600;
    text-shadow: 2px 2px 12px rgba(0,0,0,0.2);
    margin-bottom: 30px;
    animation: textPop 1.5s ease forwards;
  }

  @keyframes textPop {
    0% { transform: scale(0.8); opacity: 0; }
    100% { transform: scale(1); opacity: 1; }
  }

  .btn {
    padding: 15px 45px;
    margin: 10px;
    font-size: 1.6rem;
    border: none;
    border-radius: 20px;
    cursor: pointer;
    color: white;
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    transition: all 0.3s ease;
    opacity: 1;
  }

  .btn:hover {
    transform: scale(1.15);
    box-shadow: 0 12px 25px rgba(0,0,0,0.4);
  }

  .btn-yes {
    background: linear-gradient(45deg, #33cc33, #009900);
  }

  .btn-no {
    background: linear-gradient(45deg, #ff4d6d, #ff1a4d);
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

  <button class="btn btn-no hidden">Are you sure ?</button>
  <button class="btn btn-no hidden">Are you really sure</button>
  <button class="btn btn-no hidden">Are you really really sure</button>
  <button class="btn btn-no hidden">Think again? 😕</button>
  <button class="btn btn-no hidden">Don't believe in second chance ?</button>
  <button class="btn btn-no hidden">Why are you being so cold 🥶</button>
  <button class="btn btn-no hidden">Maybe we can talk about it ?</button>
  <button class="btn btn-no hidden">I am not going to ask again !</button>
  <button class="btn btn-no hidden">Ok now this is hurting my feelings!</button>
</div>

<script>
  const yesBtn = document.getElementById('yes');
  const noBtn = document.getElementById('no');
  const buttons = document.querySelectorAll('#buttons .btn-no');

  let index = 0; // المؤشر للزر الحالي من No options
  let yesScale = 1.2; // مقياس تكبير زر Yes

  // عند الضغط على Yes
  yesBtn.addEventListener('click', () => {
    alert('🐥🐥');
  });

  // عند الضغط على No
  noBtn.addEventListener('click', () => {
    noBtn.classList.add('hidden');
    buttons[index].classList.remove('hidden');
    yesBtn.style.transform = `scale(${yesScale})`;
    yesScale += 0.2;
  });

  // التعامل مع باقي الأزرار
  buttons.forEach((btn) => {
    btn.addEventListener('click', () => {
      // تصغير الزر الحالي تدريجيًا قبل اختفائه
      btn.style.transition = 'all 0.3s ease';
      btn.style.transform = 'scale(0.5)';
      btn.style.opacity = '0.3';
      setTimeout(() => {
        btn.classList.add('hidden');
        // إظهار الزر التالي
        index++;
        if(index < buttons.length){
          buttons[index].classList.remove('hidden');
        }
        // تكبير زر Yes تدريجيًا
        yesBtn.style.transform = `scale(${yesScale})`;
        yesScale += 0.2;
      }, 300);
    });
  });
</script>

</body>
</html>
