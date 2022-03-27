uses graphABC;
var x1,y1,x2,y2,x3,y3,x4,y4:integer;
    cl,op:boolean;
begin
  SetWindowWidth(1920);
  SetWindowHeight(1000);
  SetWindowLeft(-9);
  SetWindowTop(0);
  
  //head
  circle(960,540,400);
  
  //mouth
  arc(960,540,300,180,360);
  
  //eyes
  x1:=700;
  y1:=280;
  x2:=820;
  y2:=400;
  x3:=1100;
  y3:=280;
  x4:=1220;
  y4:=400;
  //blinking
  cl:=true;
  op:=false;
  while 2>1 do begin
    Ellipse(x1,y1,x2,y2);
    Ellipse(x3,y3,x4,y4);
    //closing eyes
    if cl=true then begin
      y1:=y1+1;
      y2:=y2-1;
      y3:=y3+1;
      y4:=y4-1;
      sleep(10);
    end;
    if y1=y2 then begin cl:=false; op:=true; end;
    //opening eyes
    if  op=true then begin
      y1:=y1-1;
      y2:=y2+1;
      y3:=y3-1;
      y4:=y4+1;
      sleep(10);
    end;
    if y1=280 then begin cl:=true; op:=false; end;
    
  end;
end.
