int startX = 150;
int startY = 0;
int endX = 50;
int endY =0;

void setup()
{
  size(300,300);
  background(0);
  strokeWeight(3);
  
}
void draw()
{
  stroke((int)(Math.random()*256), (int)(Math.random()*256),(int)(Math.random()*256),500);
  while(endX < 300)
  {
    endX = startX + (int)((Math.random()*19)-9);
    endY = startY + (int)(Math.random()*10);
    line(startX,startY,endX,endY);
    startX = endX;
    startY = endY;
  } 

}
void mousePressed()
{
  startX = 150;
  startY = 0;
  endX = 50;
  endY = 0;

}

