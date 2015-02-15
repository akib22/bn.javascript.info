Ответ: первое и третье выполнятся. 

Детали:

```js
//+ run
// Выполнится
// Результат -1 || 0 = -1, в логическом контексте true
if (-1 || 0) alert('первое'); 

// Не выполнится
// -1 && 0 = 0,  в логическом контексте false
if (-1 && 0) alert('второе'); 

// Выполнится
// оператор && имеет больший приоритет, чем ||
// так что -1 && 1 выполнится раньше
// вычисления: null || -1 && 1 -> null || 1 -> 1
if (null || -1 && 1) alert('третье');
```
