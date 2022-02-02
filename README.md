/*this in C*/
int b = 2;
  int b2 = 3;
  int c1 = 0;
  int c2 = 0;
  bool on = true;
  void setup()
  {
    Serial.begin(9600);
    pinMode(b, INPUT);
    pinMode(b2, INPUT);
  }
  
  void player1()
  {
   int bs = digitalRead(b);
   if (on == true)
    {
      Serial.println("Game begin");
    }
    else if (bs == HIGH)
      c1 = c1 + 1;
      Serial.print("Player1 = "); 
      Serial.println(c1);
      if (c1 == 10)
      {
        Serial.println("Player1 Wins");
      {
      } 
    }
  }
  void player2()
  {
   int bs2 = digitalRead(b2);
    if (on == true)
    {
      Serial.println("Game begin");
    }
    else if (bs2 == HIGH)
      c2 = c2 + 1;
      Serial.print("Player2 = "); 
      Serial.println(c2);
      if (c2 == 10)
      {
        Serial.println("Player2 Wins");
      {
      } 
    }
  }
