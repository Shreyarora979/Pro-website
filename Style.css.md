/* Import a cute font */  
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap');  
  
body {  
    font-family: 'Arial', sans-serif;  
    background: linear-gradient(135deg, #ffb3ba, #ffdfba, #ffffba, #baffc9, #bae1ff); /* Soft rainbow pastel gradient */  
    color: #333;  
    text-align: center;  
    margin: 0;  
    padding: 50px;  
    overflow-x: hidden; /* Prevent horizontal scroll */  
}  
  
.hearts-bg {  
    position: fixed;  
    top: 0;  
    left: 0;  
    width: 100%;  
    height: 100%;  
    background-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><text y="50%" font-size="20" fill="%23ff69b4" opacity="0.1">💖</text></svg>');  
    background-size: 50px 50px;  
    animation: float 10s infinite linear;  
    z-index: -1; /* Behind content */  
}  
  
@keyframes float {  
    0% { transform: translateY(0); }  
    100% { transform: translateY(-100px); }  
}  
  
.container {  
    max-width: 650px;  
    margin: 0 auto;  
    background: rgba(255, 255, 255, 0.95);  
    padding: 50px;  
    border-radius: 20px;  
    box-shadow: 0 10px 30px rgba(255, 105, 180, 0.3); /* Pink shadow for cuteness */  
    position: relative;  
    animation: bounce-in 1s ease-out;  
}  
  
@keyframes bounce-in {  
    0% { transform: scale(0.8); opacity: 0; }  
    50% { transform: scale(1.05); }  
    100% { transform: scale(1); opacity: 1; }  
}  
  
h1, h2 {  
    font-family: 'Dancing Script', cursive; /* Cuter, handwritten-style font */  
    color: #ff69b4; /* Hot pink */  
    font-size: 2.5em;  
    margin-bottom: 20px;  
}  
  
p {  
    font-size: 1.2em;  
    line-height: 1.6;  
    margin: 20px 0;  
}  
  
.cute-btn {  
    background: linear-gradient(45deg, #ff69b4, #ffb6c1); /* Gradient pink */  
    color: white;  
    border: none;  
    padding: 15px 30px;  
    font-size: 20px;  
    font-weight: bold;  
    border-radius: 50px; /* Rounded for cuteness */  
    cursor: pointer;  
    margin: 15px;  
    box-shadow: 0 5px 15px rgba(255, 105, 180, 0.4);  
    transition: all 0.3s ease;  
}  
  
.cute-btn:hover {  
    transform: scale(1.1);  
    box-shadow: 0 8px 20px rgba(255, 105, 180, 0.6);  
}  
  
.hidden {  
    display: none;  
}  
  
.fade-in {  
    animation: fade-in 1s ease-in;  
}  
  
@keyframes fade-in {  
    from { opacity: 0; transform: translateY(20px); }  
    to { opacity: 1; transform: translateY(0); }  
}  
  
/* Mobile tweaks for cuteness */  
@media (max-width: 600px) {  
    .container { padding: 30px; }  
    h1, h2 { font-size: 2em; }  
    .cute-btn { padding: 12px 25px; font-size: 18px; }  
}  
