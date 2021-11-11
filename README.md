# Nyah
'Do Not Push' project proposal


Motivation:

I want to create a unique and constantly changing art piece which acts as a platform to inspire and boost creativity in a community. 


Description:

I will be proposing a generative art piece. I would install a red button with a sign reading ‘Do not push’, assuming people will then 
be tempted to push the button. This button would alter the generative art every time it gets pressed. The person pressing the button 
will be able to see these changes on a screen in front of them. The person can chose to press the button as many times as they want or 
not at all. Allowing a random factor to contribute to the art. This project relates to the creative computing we’ve been learning because 
the Arduino board would act as the red button sensor. 


Installation:

This could be installed in any public area but would probably be the most successful on csm campus or in a gallery / exhibition space.


Red Button Coding:

/* 
DIY Code Red Button 
Created by David Escobar 
Date: 04/14/17 
*/ 

int ledOn = 4; //LED Button On
int led1 = 5; //LED 1 
int led2 = 6; //LED 2 
int led3 = 7; //LED 3 

void setup() { 
	pinMode(ledOn, OUTPUT); 
	pinMode(led1, OUTPUT); 
	pinMode(led2, OUTPUT); 
	pinMode(led3, OUTPUT);
 } 

void loop() { 

	blink(); 
} 
void blink(){
	digitalWrite(ledOn, HIGH); 
	digitalWrite(led1, HIGH); 
	digitalWrite(led2, HIGH); 
	digitalWrite(led3, HIGH); 
	delay(250); 	
	digitalWrite(led1, LOW); 
	digitalWrite(led2, LOW); 
	digitalWrite(led3, LOW); 
	delay(100);
}
