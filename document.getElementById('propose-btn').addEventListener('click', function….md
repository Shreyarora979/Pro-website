document.getElementById('propose-btn').addEventListener('click', function() {  
    const proposal = document.getElementById('proposal');  
    proposal.classList.remove('hidden');  
    // Add a cute delay for effect  
    setTimeout(() => proposal.classList.add('fade-in'), 100);  
});  
  
document.getElementById('yes-btn').addEventListener('click', function() {  
    // Trigger confetti explosion!  
    confetti({  
        particleCount: 100,  
        spread: 70,  
        origin: { y: 0.6 }  
    });  
    alert('Yay! I love you so much! 💍💕');  
});  
  
document.getElementById('no-btn').addEventListener('click', function() {  
    alert('Just kidding! Of course you say yes! 😉💖');  
});  
