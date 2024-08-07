# Содержание
- [[#Ссылки]]
	- [[#^rare|внутренние через двойные]]
	- [[#^5737d6|общий вариант]]
	- [[[#^8fd997|общий пример на внешний ресурс]]
	- [[#^8a0464|встраивание с добавлением !]]
	- [[#^904520|встраивание с добавлением ! общий]]
	- [[#^5cb824|iframe]]
-  [[#Форматирование текста]]
	- [[#Курсив]]
	- [[#Жирный]]
	- [[#Зачеркнутый]]
	- [[#Подсвеченный]]
- [[#Списки]]
	- [[#Нумерованный]]
	- [[#Точечный]]
	- [[#Список дел]]
- [[#Цитаты]]
- [[#Встраивание кода]]
	- [[#Блочно]]
	- [[#Строчно]]
- [[#Сноски]]
- [[#Мат формулы]]
- [[#Комментарии]]



---
## Ссылки


[[test_case/README|'|'отвечает за текст заменяемый]] - ссылка на документ внутри [[]] ^rare

[тоже самое](test_case/README.md) ^5737d6

[ссылка на внешний ресурс](https://habr.com/ru/companies/inpglobal/articles/722792/)  ^8fd997

![[test_case/Шпаргалка по Markdown#Форматирование текста]]

![[test_case/README|только встраивает]] ^8a0464

пауза

![название](test_case/README.md) ^904520

<iframe src="https://publish.obsidian.md/help-ru/Руководства/Встраивание+вложений+в+заметки"></iframe>

^5cb824


---

## Форматирование текста

### Курсив
*курсивный текст*
_аналог тоже курсив_

### Жирный 

**жирный текст**
__аналог жирного текста__


### Зачеркнутый
~~что-то~~

### Подсвеченный

==подсвеченный==

---

## Списки

### Нумерованный 

1. Один
2. Два
	1. Следующий уровень

### Точечный

- Первый
- Второй
	- Второй уровень
		1. Комбинация

### Список дел

- [x] Первое
- [ ] Второе
1. [ ] Нумерованное не работает
2. [ ] След

## Встраивание кода

### Строчно
`оформление кодом`

### Блочно 

```js
function name(kargo){
let b=kargo;
}
```


## Сноски


Текст[^1], который отправляет на короткую сноску
Текст[^2], который отправляет на длинную сноску


[^1]: со смыслом!

[^2]: с несколькими абзацами и кодом. 
			Делайте отступ перед абзацем, чтобы включить его в сноску. 
			`{ мой код }` 
			Абзацев может быть сколько угодно.



## Мат формулы

Для отображения формулы в отдельном блоке, необходимо заключить ее в двойные `$$`:

```md
$$\begin{vmatrix}a & b\\
c & d
\end{vmatrix}=ad-bc$$
```
$$\begin{vmatrix}a & b\\
c & d
\end{vmatrix}=ad-bc$$

## Комментарии

%%текст не виден%% теперь виден


## Цитаты 


> Текст цитаты 

\- Автор цитаты