| Задание | JS |
| --- | --- |
| 1. Создать переменную “item_1”<br>2. Присвоить переменной item_1 цифру 5. | let item_1 = 5; |
| 3. Вывести в консоль item_1. | console.log(item_1); |
| 4. Создать переменную “item_2”<br>5. Присвоить переменной item_2 цифру 3. | let item_2 = 3; |
| 6. Вывести в консоль item_2. | console.log(item_2); |
| 7. Создать переменную “item_3”<br>8. Присвоить переменной item_3 сложение item_1 и item_2. | let item_3 = item_1 + item_2; |
| 9. Вывести в консоль item_3. | console.log(item_3); |
| 10. Создать переменную “item_4”<br>11. Присвоить переменной item_4 строку “Yolochka” | let item_4 = "Yolochka"; |
| 12. Вывести в консоль item_4. | console.log(item_4);
| 13. Вывести в консоль сложение item_3 и item_4. | console.log(item_3 + item_4);
| 14. Вывести в консоль умножение item_3 и item_4. | console.log(item_3 * item_4); 
| 15. Создать переменную “item_5”<br>16. Присвоить переменной item_5 переменную item_3 | let item_5 = item_3;
| 17. Создать переменную item_6. | let item_6;
| 18. Создать переменную item_6_type | let item_6_type;  
| 19. Присвоить переменной item_6 значение 15 | item_6 = 15; 
| 20. Присвоить переменной item_6_type тип переменной item_6 | item_6_type = typeof item_6;  
| 21. Вывести в консоль тип данных item_6 в виде ——  “item_6 == ”  item_6,  “item_6_type == ”  item_6_type —— | console.log("item_6 == " + item_6, "item_6_type == " + item_6_type);
| 22. Создать переменную item_7 и в ней преобразовать item_6 в String. | let item_7 = String(item_6); 
| 23. Создать переменную item_7_type<br>24. Присвоить переменной item_7_type тип переменной item_7 | let item_7_type = typeof item_7;
| 25. Вывести в консоль тип данных item_7 в виде ——  “item_7 == ”  item_7,  “item_7_type == ”  item_7_type —— | console.log("item_7 == " + item_7, "item_7_type == " + item_7_type); 
| 26. Создать переменную “age_1” и присвоить ей значение 10 | let age_1 = 10; 
| 27. Создать переменную “age_2” и присвоить ей значение 18 | let age_2 = 18; 
| 28. Создать переменную “age_3” и присвоить ей значение 60 | let age_3 = 60;  
| 29. Создать if в котором будите проверять значение переменной age_1<br>30. Если age_1 < age_2, вывести в консоль “You don’t have access cause your age is ” + age_1 + “ It’s less then ” + age_2 | if (age_1 < age_2) {console.log("You don’t have access cause your age is " + age_1 + " It’s less then " + age_2)} 
| 31. Если age_1 >=  age_2 и age_1 <  age_3, вывести в консоль “Welcome!” | else if (age_1 >=  age_2 && age_1 < age_3){console.log("Welcome!")} 
| 32. Если age_1  > age_3, вывести в консоль “Keep calm and look Culture channel”. | else if (age_1  > age_3){console.log("Keep calm and look Culture channel")} 
| 33. Иначе выводите “Technical work”. | else {console.log("Technical work")}; 



**OUTPUT**  
[Running] node "f:\Testing\launch.json\HW_1.js"  
5  
3  
8  
Yolochka  
8Yolochka  
NaN  
item_6 == 15 item_6_type == number  
item_7 == 15 item_7_type == string  
You don’t have access cause your age is 10 It’s less then 18  


| Задания со * | JS | OUTPUT
|--- | --- | ---
| 1*. Преобразовать написанный код в 26-33 пунктах в функцию, принимающую на вход возраст.<br>Пример: const checkAge = function(age) {<br>Ваши преобразования<br>}<br>Вывести в консоль результат работы функции с возрастами 17, 18, 61 | const checkAge = function(age) {<br>const age_2 = 18;<br>const age_3 = 60;<br>if (age < age_2) {console.log("You don’t have access cause your age is " + age + " It’s less then " + age_2)}<br>else if (age >=  age_2 && age < age_3){console.log("Welcome!")}<br>else if (age  > age_3){console.log("Keep calm and look Culture channel")}<br>else {console.log("Technical work")};<br>}<br>checkAge(17);<br>checkAge(18);<br>checkAge(61); | [Running] node "f:\Testing\launch.json\HW_1.js"<br>You don’t have access cause your age is 17 It’s less then 18<br>Welcome!<br>Keep calm and look Culture channel
| 2*. Преобразовать задание 1* таким образом, чтобы первым делом в функции проверялся тип данных. И если он не Number - кидалась ошибка. | const checkAge = function(age) {<br>const age_2 = 18;<br>const age_3 = 60;<br>if (typeof age !== 'number') {<br>console.log("Error: age should be a number");<br>}else if (age < age_2) {console.log("You don’t have access cause your age is " + age + " It’s less then " + age_2)}<br>else if (age >=  age_2 && age < age_3){console.log("Welcome!")}<br>else if (age  > age_3){console.log("Keep calm and look Culture channel")}<br>else {console.log("Technical work")};<br>}<br>checkAge(17);<br>checkAge(18);<br>checkAge(61);<br>checkAge("Twenty"); | [Running] node "f:\Testing\launch.json\HW_1.js"<br>You don’t have access cause your age is 17 It’s less then 18<br>Welcome!<br>Keep calm and look Culture channel<br>Error: age should be a number
| 3**. Преобразовать 2* таким образом, чтобы значение '2' (строка в которой лежит ТОЛЬКО ЦИФРА) пропускалось, преобразовываясь в number | const checkAge = function(age) {<br>const age_2 = 18;<br>const age_3 = 60;<br>   if (typeof age !== 'number') {<br>age = Number(age)};<br>if (age < age_2) {console.log("You don’t have access cause your age is " + age + " It’s less then " + age_2)}<br>else if (age >=  age_2 && age < age_3){console.log("Welcome!")}<br>else if (age  > age_3){console.log("Keep calm and look Culture channel")}<br>else {console.log("Technical work")};<br>}<br>checkAge(17);<br>checkAge(18);<br>checkAge(61);<br>checkAge("20"); | [Running] node "f:\Testing\launch.json\HW_1.js"<br>You don’t have access cause your age is 17 It’s less then 18<br>Welcome!<br>Keep calm and look Culture channel<br>Welcome!
| 4***. Преобразовать задание 3* таким образом, чтобы возраст вводится используя функцию prompt в привязанной верстке | const checkAge = function() {<br>const age_2 = 18;<br>const age_3 = 60;<br>let age = prompt("Enter your age");<br>age = Number(age);<br>if (age < age_2) {console.log("You don’t have access cause your age is " + age + " It’s less then " + age_2)}<br>else if (age >=  age_2 && age < age_3){console.log("Welcome!")}<br>else if (age  > age_3){console.log("Keep calm and look Culture channel")}<br>else {console.log("Technical work")};<br>}<br>checkAge();
