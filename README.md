# Zamasor.github.io

// Definição dos pinos para as cores do LED RGB
const int pinRed = 9;
const int pinGreen = 10;
const int pinBlue = 11;

// Função para definir a cor do LED
void setColor(int red, int green, int blue) {
    analogWrite(pinRed, red);
    analogWrite(pinGreen, green);
    analogWrite(pinBlue, blue);
}

void setup() {
    pinMode(pinRed, OUTPUT);
    pinMode(pinGreen, OUTPUT);
    pinMode(pinBlue, OUTPUT);
}

void loop() {
    setColor(255, 0, 0); // Vermelho
    delay(1000);
    setColor(0, 255, 0); // Verde
    delay(1000);
    setColor(0, 0, 255); // Azul
    delay(1000);
    setColor(255, 255, 0); // Amarelo
    delay(1000);
    setColor(0, 255, 255); // Ciano
    delay(1000);
    setColor(255, 0, 255); // Magenta
    delay(1000);
    setColor(255, 255, 255); // Branco
    delay(1000);
}