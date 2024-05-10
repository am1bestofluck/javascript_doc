### live server для Visual studio code
* где ставить скрипт на html-странице	в конце, на строке перед </body>
* способы подключить js	* вписать прямо в html * подключить файл
* как подключить файл	```<script src="path/to.js"></script>```
* почему не пользуем alert("no!");	блокируется выполнение страницы; хуже чем developer tools[console]
* очищаем консоль devtools 	console.clear();
* выводим без блокировки страницы в консоль	console.log('right!');
* объявление переменных(3) 	var,let,const
* комментарий в js	// так
* особенность переменных var	они глобальные, так - может возникнуть конфликт имён между этажами
* разница между let и const 	переменные let можно переназначать, а const - константы;
* переназначаем переменную 	let b; let a = 1; a = 2;, т.е. ключ- объявления даём только в первый раз.
* стратегия выбора между let и const("надёжная")	используем const, кроме случаев что Мы точно знаем что переменную будем менять
* особенность const для коллекций 	можно менять объект поэлементно, нельзя назначить другой объект
* простые типы данных 	strings,numbers,Boolean, null, undefined, Symbol
* обрамление strings	'',"" как двойные так и одинарные кавычки
* роль точкозапятых 	желательны но опциональны
* получаем тип переменной	console.log(typeof(var_name));
* почему typeof(null) возвращает не null	обратная совместимость с первой версией js;
* Обработка составных строк(2)	конкатенация( 'сложение '+2+' строк') и Template Strings(`Сложение ${amount} строк;`);
* отличие свойства объекта от метода объекта 	свойство вызывается без скобок/* передачи аргументов */, н. some_str.length, some_str.toUpperCase()
* цепной вызов методов 	Hello_str.substring(0,5).toUpperCase();
* дробим строку 	some_str.split(''), где агрумент split - знак делитель;
* создаём массив(2) 	const nums = new Array(1,2,34); const letters = ['q','w'];
* Read к элементу массива(2)	console.log(arr[0]); arr.indexOf('here');
* Update к элементу массива 	const arr = [1,2]; arr[2]=3; arr.push(4); arr.push(0);
* разница arr.push arr.unshift 	push добавляет в конец списка; unshift в начало
* Delete к элементу массива 	const arr = [1,23,45,6]; arr.pop()
* словари/object literals create	const it_s_dict = {keys:0,unframed:['h','ere']};
* словари/object literals read 	console.log(it_s_dict.unframed[0],it_s_dict.unframed[1]); обращение к ключам через точку
* создаём отдельную переменную из словаря 	const {unframed } = it_s_dict;
* вынимаем переменную из вложенного словаря 	const b4 ={other:'stuff',nest:{eggs:4,birds:2}}; const {nest: {birds}} = b4 ; console.log(birds)/* 2 */;
* словари/object literals update 	const later ={}; later.finally=True;
* переводим object literal в json 	const new_json =JSON.stringify(later)
* цикл for 	for (let i = 0; i < 10; i++) {console.log(i);}
* цикл while 	let i = 0; while ( i<10){ console.log(`#$(i)`); i++;}
* проходы по списку(2)	for (let i=0; i < arr.length; i++ ) {console.log(arr[i])}; for (let item of arr){ console.log(item);}
* кавычки в json 	только двойные, вокруг ключей и строк-значений