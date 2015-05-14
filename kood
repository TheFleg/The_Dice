//Arduino kood Egerti, Laura ja Kaarli poolt
//LED täring

//Ledi pinnid
int pinLeds1 = 10;
int pinLeds2 = 9;
int pinLeds3 = 8;
int pinLed4 = 7;
//Button pin
int buttonPin = 6;
int buttonState;
//Veeretused tulevad suvaliselt ühest kuueni
long ran;
//Viivitus
int time = 2000;

void setup ()
{
  //Ledi pinnid lähevad väljundisse
  pinMode (pinLeds1, OUTPUT);
  pinMode (pinLeds2, OUTPUT);
  pinMode (pinLeds3, OUTPUT);
  pinMode (pinLed4, OUTPUT);
  //Nupp pinni sisendiks
  pinMode (buttonPin, INPUT);
  //Kood korrekteerib juhuslikkust
  randomSeed(analogRead(0));
}

void loop()
{
  //Nupu staatuse lugemine
  buttonState = digitalRead(buttonPin);
  if (buttonState == HIGH){
	//Suvaliselt ühest kuueni
	ran = random(7);
	//Number üks
	if (ran == 1){
  	digitalWrite (pinLed4, HIGH);
  	delay (time);
	}
	//Number kaks
	if (ran == 2){
  	digitalWrite (pinLeds1, HIGH);
  	delay (time);
	}
	//Number kolm
	if (ran == 3){
  	digitalWrite (pinLeds3, HIGH);
  	digitalWrite (pinLed4, HIGH);
  	delay (time);
	}
	//Number neli
	if (ran == 4){
  	digitalWrite (pinLeds1, HIGH);
  	digitalWrite (pinLeds3, HIGH);
  	delay (time);
	}
	//Number viis
	if (ran == 5){
  	digitalWrite (pinLeds1, HIGH);
  	digitalWrite (pinLeds3, HIGH);
  	digitalWrite (pinLed4, HIGH);
  	delay (time);
   }
   //Number kuus
   if (ran == 6){
  	digitalWrite (pinLeds1, HIGH);
  	digitalWrite (pinLeds2, HIGH);
  	digitalWrite (pinLeds3, HIGH);
  	delay (time);
   }
  }
  //Kui nuppu ei vajuta, siis ledid põlema ei lähe
  digitalWrite (pinLeds1, LOW);
  digitalWrite (pinLeds2, LOW);
  digitalWrite (pinLeds3, LOW);
  digitalWrite (pinLed4, LOW);
}

//Kõik!


