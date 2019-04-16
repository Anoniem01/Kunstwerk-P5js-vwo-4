var ypos = 40 // y positie van het vierkantje
var xpos = 40 // x positie van het vierkantje
var xstep = 80 // afstand tussen de vierkantjes
var ystep = 80 // afstand tussen vierkantjes
var x = 100

function setup() {
  createCanvas(480, 480); // maakt een doek waarop getekent word van 480 bij 480
  rectMode(CENTER); // zorgt er voor dat de vierkantjes om het midden heen draaien
}

function draw() {

  background(0, 255, 0) // maakt de achtergrond groen

  for (var kolom = 0; kolom < 6; kolom++) { // als de kolom kleiner is dan 6 teken dan nog een     vierkantje 
    for (var rij = 0; rij < 6; rij++) { // als de rij kleiner is dan 6 teken dan nog een vierkantje 

      push()

      translate(xpos + (xstep * kolom), ypos + (ystep * rij))
      rotate(frameCount / 40); // bepaalt hoe snel de vierkantjes draaien
      if (kolom < 3) {

        if (rij < 3) { // als de kolom en rij kleiner is dan 3 kleur rood


          fill(255, 0, 0); // kleur van de vierkantjes links boven

        } else { // anders kleur geel
          fill(255, 255, 0) // kleur van de vierkantjes links onder
        }
      } else {
        if (rij < 3) { // als rij is kleiner dan 3 kleur blauw


          fill(0, 255, 255); // kleur van vierkantjes rechts boven

        } else { // anders kleur roze
          fill(255, 0, 255); // kleur van vierkantjes rechts onder
        }
      }


      rect(0, 0, 50, 50) // bepaalt hoe groot de vierkantjes zijn


      pop()
    }
  }

}
