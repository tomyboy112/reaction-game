# reaction-game
its the best game in the world :)


```
float timer = 30;
float score = 0;
float tijdDatVoidDrawBegint = 0;
float hoeLangVoidDrawBezigIsInMilliseconden, hoeLangVoidDrawBezigIsInSeconden;
int plek = 0;


void setup() {
   background(143,123,213);

   
  size(1300,800);
  plek = (int)random(1, 6);
  textSize(50);
  tijdDatVoidDrawBegint = millis();
}

void draw()
{
  if(mousePressed) {
    if(dist(mouseX,mouseY,200,500) < 50 && plek == 1){
      plek = (int)random(1, 6);
      score = score +1;
    }
     if(dist(mouseX,mouseY,350,350) < 50 && plek == 2){
      plek = (int)random(1, 6);
      score = score +1;
    }
     if(dist(mouseX,mouseY,500,200) < 50 && plek == 3){
      plek = (int)random(1, 6);
      score = score +1;
    } 
    if(dist(mouseX,mouseY,700,200) < 50 && plek == 4){
      plek = (int)random(1, 6);
      score = score +1;
    }
     if(dist(mouseX,mouseY,850,350) < 50 && plek == 5){
      plek = (int)random(1, 6);
      score = score +1;
    }
     if(dist(mouseX,mouseY,1030,500) < 50 && plek == 6){
      plek = (int)random(1, 6);
      score = score +1;
    }
  }
  
 hoeLangVoidDrawBezigIsInMilliseconden =  millis()- tijdDatVoidDrawBegint ;
 hoeLangVoidDrawBezigIsInSeconden = hoeLangVoidDrawBezigIsInMilliseconden/1000  ;
 
timer = 30 - hoeLangVoidDrawBezigIsInSeconden ;
  
  if (plek == 1) { fill(20,123,55); }
  else { fill(255); }
  ellipse(200,500,100,100);
  
  if (plek == 2) { fill(20,123,55); }
  else { fill(255); }
  ellipse(350,350,100,100);
  
  if (plek == 3) { fill(20,123,55); }
  else { fill(255); }
  ellipse(500,200,100,100);

  if (plek == 4) { fill(20,123,55); }
  else { fill(255); }
  ellipse(700,200,100,100);

  if (plek == 5) { fill(20,123,55); }
  else { fill(255); }
  ellipse(850,350,100,100);

  if (plek == 6) { fill(20,123,55); }
  else { fill(255); }
  ellipse(1030,500,100,100);
  fill(227,28,41);
  rect(1100,50,200,100);
  fill(143,123,213);
  text(timer,1100,100);
fill(227,28,41);
rect(1100,150,200,100);
fill(43,123,130);
text(int(score), 1100,200);

  
  
  if (timer <= 0) 
  {  exit();
  }
}

```
