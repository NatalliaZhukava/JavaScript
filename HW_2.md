**Напишите валидационный скрипт используя функции** 

 1. Скрипт должен на вход принимать строку.
 2. После проверки строки выводить в консоль сообщение где будет конкретно написано, что не так в ведённой строке.
 3. Минимум 5 символов в строке
 4. Максимум 64 символа в строке
 5. В строке должны быть буквы
 6. Должна быть хотя бы одна буква в верхнем регистре
 7. Должна быть хотя бы одна цифра
 8. Должна быть хотя бы одна @
 9. Строка не должна быть пустой

**JS**  
function validateField(input){  
    if (input.length == 0){  
        console.log("Error: input shouldn't be empty");  
    }  
    else if (typeof input !== "string"){  
        console.log("Error: input should be a string");  
    }  
    else if (input.length < 5 || input.length > 64){  
        console.log("Error: input should be 5-64 characters");  
    }  
        else if (!/[a-zA-Z]/.test(input)) {  
        console.log("Error: input should contain at least 1 letter");  
    }  
    else if (!/[A-Z]/.test(input)) {  
        console.log("Error: input should contain at least 1 capital letter");  
    }  
    else if (!/[0-9]/.test(input)) {  
        console.log("Error: input should contain at least 1 number");  
    }  
    else if (!/[@]/.test(input)) {  
        console.log("Error: input should contain @");  
    }  
}  
  
validateField("");  
validateField(20);  
validateField("hhy");  
validateField("789800");  
validateField("789800g");  
validateField("Hgfgfdg");  
validateField("Hgfgfdg1");  

**OUTPUT**  
[Running] node "f:\Testing\launch.json\HW_2.js"  
Error: input shouldn't be empty  
Error: input should be a string  
Error: input should be 5-64 characters  
Error: input should contain at least 1 letter  
Error: input should contain at least 1 capital letter  
Error: input should contain at least 1 number  
Error: input should contain @  
