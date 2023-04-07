# my
int s=0;
int D=200;

void setup() {
  pinMode(0, INPUT_PULLUP);
  for (int i = 1; i < 11; i++) {
    pinMode(i, OUTPUT);
  }
}


void loop() {
  s = digitalRead(0);
  if (s == 0) {
    for (int i = 1; i < 11; i++){
    digitalWrite(i, HIGH);
    delay(D);
 } } else {
    for (int i = 1; i < 11; i++){
    digitalWrite(i, LOW);
    delay(D);  
    }}
 // delay(10);
}





لدینا 10 لیدات نریدھا تعمل معا ً عند الضغط على زر sw المطلوب یكون بینھا تأخیر زمني بسیط (الأول ثم
الثاني ثم الثالث وھكذا) كما أنھا تنطفئ بنفس الطریقة عند ترك الزر.
