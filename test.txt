/* BONUS : le carousel changera d'image au bout de 5 seconde */

$('.carousel').carousel({
    interval: 5000
  
  })


var listeImages = document.querySelectorAll('#barre img');

for(var img of listeImages) {
    img.addEventListener('click', function() {
        var nouveauSrc = 'image/' + this.id + '.png';
        document.getElementById('imagePrincipale').src = nouveauSrc;  
    });
}