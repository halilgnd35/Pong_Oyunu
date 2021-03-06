# Pong_Oyunu
Basit bir pong oyunu.Tanımlamaların yapıldığı pinlere ledler ve butonlar uygun şartlarda takılıp yahut tanımlamaları gereklere göre değiştirip kurulum yapıldıktan sonra oyunu oynayabilirsiniz.Oyunumuza can veren kodlar aşağıdadır.
```javascript
-----------------------Kodlar-----------------------
//Author:Halil Gundogdu
const byte ki=13;
const byte mi=12;
const byte y1=11;
const byte y2=10;
const byte y3=9;
const byte y4=8;
const byte y5=7;
const byte ms=6;
const byte ks=5;
const byte b1=4;
const byte b2=3;
 int m,n,i=1000;
 int c1=0,c2=0;
void setup()
{
  pinMode(ki, OUTPUT);
  pinMode(mi, OUTPUT);
  pinMode(y1, OUTPUT);
  pinMode(y2, OUTPUT);
  pinMode(y3, OUTPUT);
  pinMode(y4, OUTPUT);
  pinMode(y5, OUTPUT);
  pinMode(ms, OUTPUT);
  pinMode(ks, OUTPUT);
  pinMode(b1, INPUT);
  pinMode(b2, INPUT);
}
void loop()
{
 int m,n,i=1000;
 int c1=0,c2=0;
  while(1)
  {
  while(1)
  {
  digitalWrite(mi,HIGH);
  delay(i);
  if(i!=1000)
  {
   m=digitalRead(b1); //mavi sorgulama kodları
   n=digitalRead(b2);
  if(m==LOW)
  {
    digitalWrite(mi,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(mi,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  }
  delay(i);
  digitalWrite(mi,LOW);
  digitalWrite(y1,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y1,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y1,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y1,LOW);
  digitalWrite(y2,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y2,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y2,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y2,LOW);
  digitalWrite(y3,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y3,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y3,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y3,LOW);
  digitalWrite(y4,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y4,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y4,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y4,LOW);
  digitalWrite(y5,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y5,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y5,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y5,LOW);
  digitalWrite(ms,HIGH);
  delay(i);
   m=digitalRead(b1); //mavi sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(ms,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==LOW)
  {
    digitalWrite(ms,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }
  delay(i);//sabitlerin bitişi
  digitalWrite(ms,LOW);
 digitalWrite(y5,HIGH); //geriye dönüşün başlangıcı
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y5,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y5,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y5,LOW);
digitalWrite(y4,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y4,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y4,LOW);
c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y4,LOW);
digitalWrite(y3,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y3,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y3,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y3,LOW);
digitalWrite(y2,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y2,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y2,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y2,LOW);
 digitalWrite(y1,HIGH);
  delay(i);
   m=digitalRead(b1); //sabit sorgulama kodları
   n=digitalRead(b2);
  if(m==HIGH)
  {
    digitalWrite(y1,LOW);
    c2=c2+1;
    digitalWrite(ki,HIGH);
    break;
  }
  if(n==HIGH)
  {
    digitalWrite(y1,LOW);
    c1=c1+1;
    digitalWrite(ks,HIGH);
    break;
  }                    //sabitlerin bitişi
  delay(i);
  digitalWrite(y1,LOW);
  i=i/2;
}
i=1000;
if(digitalRead(ki)==HIGH)
{
delay(1000);
digitalWrite(ki,LOW);
delay(500);
digitalWrite(ki,HIGH);
delay(500);
digitalWrite(ki,LOW);
delay(500);
digitalWrite(ki,HIGH);
delay(500);
digitalWrite(ki,LOW);
delay(500);
digitalWrite(ki,HIGH);
delay(500);
digitalWrite(ki,LOW);
  }
  else if(digitalRead(ks)==HIGH)
  {
  delay(1000);
digitalWrite(ks,LOW);
delay(500);
digitalWrite(ks,HIGH);
delay(500);
digitalWrite(ks,LOW);
delay(500);
digitalWrite(ks,HIGH);
delay(500);
digitalWrite(ks,LOW);
delay(500);
digitalWrite(ks,HIGH);
delay(500);
digitalWrite(ks,LOW);
  }
  if(c1==1&&c2==0)
  {
    digitalWrite(y1,HIGH); //skor belirtme kodları
    delay(500);
    digitalWrite(y1,LOW);
    delay(250);
    digitalWrite(y1,HIGH);
    delay(500);
    digitalWrite(y1,LOW);
    }
    else if(c1==2&&c2==0)
    {
       digitalWrite(y1,HIGH); //skor belirtme kodları
       digitalWrite(y2,HIGH);
       delay(500);
       digitalWrite(y1,LOW);
       digitalWrite(y2,LOW);
       delay(250);
       digitalWrite(y1,HIGH);
       digitalWrite(y2,HIGH);
       delay(500);
       digitalWrite(y1,LOW);
       digitalWrite(y2,LOW);
      }
      else if(c1==0&&c2==1)
      {
         digitalWrite(y5,HIGH); //skor belirtme kodları
         delay(500);
         digitalWrite(y5,LOW);
         delay(250);
         digitalWrite(y5,HIGH);
         delay(500);
         digitalWrite(y5,LOW);
        }
        else if(c1==0&&c2==2)
        {
          digitalWrite(y5,HIGH); //skor belirtme kodları
          digitalWrite(y4,HIGH);
          delay(500);
          digitalWrite(y5,LOW);
          digitalWrite(y4,LOW);
          delay(250);
          digitalWrite(y5,HIGH);
          digitalWrite(y4,HIGH);
          delay(500);
          digitalWrite(y5,LOW);
          digitalWrite(y4,LOW);
          }
          else if(c1==1&&c2==1)
          {
            digitalWrite(y5,HIGH); //skor belirtme kodları
            digitalWrite(y1,HIGH);
            delay(500);
            digitalWrite(y5,LOW);
            digitalWrite(y1,LOW);
            delay(250);
            digitalWrite(y5,HIGH);
            digitalWrite(y1,HIGH);
            delay(500);
            digitalWrite(y5,LOW);
            digitalWrite(y1,LOW);
            }
           else if(c1==2&&c2==2)
           {
            digitalWrite(y5,HIGH); //skor belirtme kodları
            digitalWrite(y1,HIGH);
            digitalWrite(y4,HIGH);
            digitalWrite(y2,HIGH);
            delay(500);
            digitalWrite(y5,LOW);
            digitalWrite(y1,LOW);
            digitalWrite(y4,LOW);
            digitalWrite(y2,LOW);
            delay(250);
            digitalWrite(y5,HIGH);
            digitalWrite(y1,HIGH);
            digitalWrite(y4,HIGH);
            digitalWrite(y2,HIGH);
            delay(500);
            digitalWrite(y5,LOW);
            digitalWrite(y1,LOW);
            digitalWrite(y4,LOW);
            digitalWrite(y2,LOW);
              }
             else if(c1==1&&c2==2)
             {
            digitalWrite(y5,HIGH); //skor belirtme kodları
            digitalWrite(y1,HIGH);
            digitalWrite(y4,HIGH);
            delay(500);
            digitalWrite(y5,LOW);
            digitalWrite(y1,LOW);
            digitalWrite(y4,LOW);
            delay(250);
            digitalWrite(y5,HIGH);
            digitalWrite(y1,HIGH);
            digitalWrite(y4,HIGH);
            delay(500);
            digitalWrite(y5,LOW);
            digitalWrite(y1,LOW);
            digitalWrite(y4,LOW);
              }
              else if(c1==2&&c2==1)
              {
            digitalWrite(y5,HIGH); //skor belirtme kodları
            digitalWrite(y1,HIGH);
            digitalWrite(y2,HIGH);
            delay(500);
            digitalWrite(y5,LOW);
            digitalWrite(y1,LOW);
            digitalWrite(y2,LOW);
            delay(250);
            digitalWrite(y5,HIGH);
            digitalWrite(y1,HIGH);
            digitalWrite(y2,HIGH);
            delay(500);
            digitalWrite(y5,LOW);
            digitalWrite(y1,LOW);
            digitalWrite(y2,LOW);
                }
                else if(c1==3)
                {
                digitalWrite(mi,HIGH);
                digitalWrite(ks,HIGH);
                delay(2500);
                digitalWrite(mi,LOW);
                digitalWrite(ks,LOW);
                delay(1000);
                digitalWrite(mi,HIGH);
                digitalWrite(ks,HIGH);
                 delay(3000);
                digitalWrite(mi,LOW);                                                                           
                digitalWrite(ks,LOW);
                break;
                }
                else if(c2==3)
                {
                digitalWrite(ms,HIGH);
                digitalWrite(ki,HIGH);
                delay(2500);
                digitalWrite(ms,LOW);
                digitalWrite(ki,LOW);
                delay(1000);
                digitalWrite(ms,HIGH);
                digitalWrite(ki,HIGH);
                delay(3000);
                digitalWrite(ms,LOW);
                digitalWrite(ki,LOW);
                break;
                }
                
  }
}
```
