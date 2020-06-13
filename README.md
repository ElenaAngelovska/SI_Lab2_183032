# Втора лабораториска вежба по Софтверско инженерство

## Елена Ангеловска, бр. на индекс 183032

### Група на код: 

Ја добив групата на код 4

###  Control Flow Graph

![ ](https://drive.google.com/file/d/1nCQ6DqJRBpR6s1rEgItTGUZB8abWEnfg/view?usp=sharing)

### Цикломатска комплексност

Цикломатската комплексност на овој код е 10, истата ја добив преку формулата P+1, каде што P е бројот на предикатни јазли. Во случајoв P=9, па цикломатската комплексност изнесува 10.

### Тест случаи според критериумот  Every branch 
   Со еvery branch е потребно да се изминат сите гранки во ЦФГ. За да се изминат сите јазли јас користам 5 тест примери прикажани во табелата.
   1.user==null
   2.user( / ,"password","email")
   3.user("Elena","cat","email@yahoo.com")
   4.user("Elena", "angelovska","email@yahoo.com")
   5.user("Elena", "Angelovska8^","email@gmail.com")
![Ова се тест примерите за Every branch пеикажани во табела ](https://drive.google.com/file/d/1vBZziB0R7uKq5kQa0r0M6GShgkN8rRjq/view?usp=sharing)

### Тест случаи според критериумот Multiple condition
## 1. if (user.getUsername()!=null && user.getPassword()!=null)
Т и Т=Т
-Двата услови во исто време треба да бидат точни што значи дека user треба да има и Username и Password. Тест пример би бил: user(“Elena”, “angelovska”, “email@gmail.com”).
## 2.  if (!passwordLower.contains(user.getUsername().toLowerCase()) && password.length()>=8)
Т и Т=Т
-И во овој multiple condition двата услови истовремено треба да бидат исполнети, password-от да не го содржи username-от и password-от да биде со 8 или повеќе карактери. Тест пример би бил  user(“Elena”, “angelovska”, “email@gmail.com”).
## 3.   if (digit && upper && special)
Т и Т и Т = Т
-Овој multiple condition е составен од три услови и сите треба да бидат исполнети. Во кодот овие три услови за да бидат true треба да исполнат други услови и во овој услов се проверува дали сите се исполнети. Тоа би значело passwordot да содржи голема бројка, голема буква и специјален знак. Тест пример би бил user(“Elena”,”Angelovska8^”,”email@gmail.com”).

