# CPS-researcher-test  <img src="https://ain17002254.files.wordpress.com/2017/09/3923-researchanddevelopmentbanner.jpg?w=150" />

Тестовое задание для кандидатов на должность CPS resercher.
- Пункты заданий расположены в порядке возрастания сложности. Выполнять можно любое понравившееся задание, столько пунктов, сколько сможете/захотите.
- Предпочтительно решать задачи, используя Python3 (и любой фреймворк для работы с нейросетями).
- Рассуждения по решению аналитических заданий можно оформить от руки, но желательно представить результаты в PDF с оформленным выводом (LaTeX или MathType).
- Каждое задание относится к тому или иному разделу машинного обучения или математического моделирования. Помимо решения задачи необходимо рассмотреть какую-либо статью, вышедшую в последние полгода на тему, связанную с заданием, и предложить как можно было бы использовать результаты этой статьи для решения данной задачи или анологичных данной.

## 1. Задание с теоретико-математическим смещением. (Оптимизация)

Заданы две функции:

<a href="https://latex.codecogs.com/gif.latex?f_1%28x%2Cy%29%3D%5Cfrac%7B1%7D%7B2%7D-%5Cfrac%7B%5Csin%5E2%28%5Csqrt%7Bx%5E2&plus;y%5E2%7D%29-%5Cfrac%7B1%7D%7B2%7D%7D%7B1&plus;%5Cfrac%7Bx%5E2&plus;y%5E2%7D%7B1000%7D%7D%20%2C%20x%2Cy%20%5Cin%20%5Cmathbb%7BR%7D" target="_blank">

<img src="https://latex.codecogs.com/gif.latex?f_1%28x%2Cy%29%3D%5Cfrac%7B1%7D%7B2%7D-%5Cfrac%7B%5Csin%5E2%28%5Csqrt%7Bx%5E2&plus;y%5E2%7D%29-%5Cfrac%7B1%7D%7B2%7D%7D%7B1&plus;%5Cfrac%7Bx%5E2&plus;y%5E2%7D%7B1000%7D%7D%20%2C%20x%2Cy%20%5Cin%20%5Cmathbb%7BR%7D"  />
</a>

     

<a href="https://latex.codecogs.com/gif.latex?f_2%28z%29%3D%5Cfrac%7B1%7D%7B1%26plus%3B%7Cz%5E6-1%7C%7D%26space%3B%2C%26space%3Bz%26space%3B%5Cin%26space%3B%5Cmathbb%7BC%7D%2Cz%3Dx%26plus%3Biy%26space%3B" target="_blank">
 
<img src="https://latex.codecogs.com/gif.latex?f_2%28z%29%3D%5Cfrac%7B1%7D%7B1%26plus%3B%7Cz%5E6-1%7C%7D%26space%3B%2C%26space%3Bz%26space%3B%5Cin%26space%3B%5Cmathbb%7BC%7D%2Cz%3Dx%26plus%3Biy%26space%3B" title="$$f_2(z)=\frac{1}{1+|z^6-1|} , z \in \mathbb{C},z=x+iy $$" />
</a>

- Найти аналитически глобальные максимумы этих функций.
- Построить графики этих функций.
- Представив, что функции являются исследуемым объектом, без аналитической формы задания (чёрный ящик), найти максимумы функций с помощью какого-либо численного метода. (Метод не обязательно нужно писать самому, можно использовать библиотечный).
- Для второй функции найти кратчайший путь по поверхности функции из одного максимума в любой другой аналитически или численно.

## 2. Задание с теоретико-математическим смещением. (Теория игр. Обучение с подкреплением. Моделирование.)

Задана следующая ситуация:
В центре круглого плоского бассейна плавает ученик. Внезапно к бассейну подошёл учитель. Учитель не умеет плавать, но бегает в 4 раза быстрее, чем ученик плавает. Ученик бегает быстрее в 4 раза когда находится на земле. В начальный момент времени ученик находится в центре бассейна. Учитель хочет поймать ученика и для этого выбирает следующую стратегию: если ученик на замле, то учитель бежит по направлению к нему, если ученик в воде, то учитель бегает по краю бассейна, бежит учитель по наименьшей дуге к точке радиальной проекции на край бассейна текущего положения ученика. Известно, что ученик не может длительное время провести в воде, так что решение должно быть реализовано за конечное время. Задача ученика выбраться из бассейна за конечное время и убежать от учителя.
- Если существует выигрышная стратегия для ученика, найти её аналитически, если нет, доказать что её не существует.
- Визуализировать стратегию поведения используя простейшие примитивы.
- Решить задачу для случая неплоского бассейна.
- Запрограммировать ситуацию описанную в задаче так, чтобы ученик стал обучаемым объектом и каким либо способом обучить его. 

## 3. Задание с математико-инженерным смещением. (Анализ сигналов. Машинное обучение. Моделирование.)

Рассматривается некоторый детерминированный объект, который может быть описан дифференциальным уравнением 4-го порядка:

<a href="https://latex.codecogs.com/gif.latex?x%5E%7B%284%29%7D%26plus%3B4x%5E%7B%283%29%7D%26plus%3B2x%5E%7B%282%29%7D%26plus%3B3x%5E%7B%281%29%7D%26plus%3Bkx%5E%7B%280%29%7D%3Dg%26space%3B" target="_blank">
<img src="https://latex.codecogs.com/gif.latex?x%5E%7B%284%29%7D%26plus%3B4x%5E%7B%283%29%7D%26plus%3B2x%5E%7B%282%29%7D%26plus%3B3x%5E%7B%281%29%7D%26plus%3Bkx%5E%7B%280%29%7D%3Dg%26space%3B" title="$$x^{(4)}+4x^{(3)}+2x^{(2)}+3x^{(1)}+kx^{(0)}=g $$" />
</a>

относительно некоторой функции времени x(t) и произвольного ограниченного входного сигнала g(t). В скобочках у неизвестной функции указан порядок дифференцирования.

 <a href="https://latex.codecogs.com/gif.latex?k%3D%5Chat%7Bf%7D%282.1%29%26space%3B" target="_blank">
 <img src="https://latex.codecogs.com/gif.latex?k%3D%5Chat%7Bf%7D%282.1%29%26space%3B" title="$$k=\hat{f}(2.1) $$" />
 </a>
 
где <a href="https://latex.codecogs.com/gif.latex?%26space%3B%5Chat%7Bf%7D%26space%3B" target="_blank"><img src="https://latex.codecogs.com/gif.latex?%26space%3B%5Chat%7Bf%7D%26space%3B" title="$$ \hat{f} $$" /></a>  - непрерывная функция, которую требуется восстановить используя предоставленный набор данных `Regression_Test.json`.

- Восстановить коэффициент k и выяснить каким либо способом что происходит с системой спустя длительное время (устойчива ли система, неустойчива или стремиться к асимптотически фиксированному состоянию) если она стартует из состояния покоя (координата и все производные до 3 порядка включительно равны нулю).
- Промоделировать систему для разных воздействий g и построить графики "Воздействие - Отклик" <a href="https://latex.codecogs.com/gif.latex?%28x%28t%29%2Cg%28t%29%2Ct%29" target="_blank"><img src="https://latex.codecogs.com/gif.latex?%28x%28t%29%2Cg%28t%29%2Ct%29" title="$(x(t),g(t),t)$" /></a>.
- Восстановление закона <a href="https://latex.codecogs.com/gif.latex?%26space%3B%5Chat%7Bf%7D%28x%29%26space%3B" target="_blank"><img src="https://latex.codecogs.com/gif.latex?%26space%3B%5Chat%7Bf%7D%28x%29%26space%3B" title="$$ \hat{f}(x) $$" /></a> произвести с использование нейронной сети.

## 4. Задание на машинное обучение и программирование. (Порождающие модели. Машинное обучение.)

- Написать генератор изображений простых геометрических фигур (круг, квадрат, треугольник), который может генерировать разнообразные пиксельные ч.б. изображение фигур.
- Генератор должен использовать нейросети.
- С помощью полученного генератора написать программу, которая на вход принимает текст на русском языке, а на выходе генерирует фигуру: круг, если в тексте было больше букв "о" чем отсальных, треугольник, если больше букв "д", квадрат в ином случае.

Для облегчения работы с данными, вместо порождения фигур можно использовать порождение арабских цифр (для чего например можно использовать датасет MNIST) и порождать в третьем пунке цифру, которая больше всего раз попалась в тексте.

## 5. Задание на машинное обучение. (Классификация. Машинное обучение.)

Задан датасэт `ionosphere.arff` в котором находится описание и происхождение данных, а так же результаты авторов датасэта.
- Необходимо построить бинарный классификатор, качество которого не уступало бы качеству классификатора, полученного авторами (информация и ссылки содержатся внутря датасэта).
- Проанализируйте оригинальную [статью](https://docviewer.yandex.ru/view/403167255/?*=4j5bhtTV6gkTf03Ydarcmn9PiNh7InVybCI6Imh0dHBzOi8vd3d3LmpodWFwbC5lZHUvVGVjaERpZ2VzdC92aWV3cy9wZGZzL1YxMF9OM18xOTg5L1YxMF9OM18xOTg5X1NpZ2lsbGl0b19DbGFzcy5wZGYiLCJ0aXRsZSI6IlYxMF9OM18xOTg5X1NpZ2lsbGl0b19DbGFzcy5wZGYiLCJ1aWQiOiI0MDMxNjcyNTUiLCJ5dSI6IjkyODIzMDM1MTE1MzUxMjE3ODUiLCJub2lmcmFtZSI6dHJ1ZSwidHMiOjE1NDM0MjEzODY2OTAsInNlcnBQYXJhbXMiOiJsYW5nPWVuJm5hbWU9VjEwX04zXzE5ODlfU2lnaWxsaXRvX0NsYXNzLnBkZiZ0bT0xNTQzNDIxMzc3JnRsZD1ydSZ0ZXh0PVNpZ2lsbGl0byUyQyUyMFYuJTIwRy4lMkMlMjBXaW5nJTJDJTIwUy4lMjBQLiUyQyUyMEh1dHRvbiUyQyUyMEwuJTIwVi4lMkMlMjAlNUMlMjYlMjBCYWtlciUyQyUyMEsuJTIwQi4lMjAlMjgxOTg5JTI5LiUyMENsYXNzaWZpY2F0aW9uJTIwb2YlMjByYWRhciUyMHJldHVybnMlMjBmcm9tJTIwdGhlJTIwaW9ub3NwaGVyZSUyMHVzaW5nJTIwbmV1cmFsJTIwbmV0d29ya3MuJTIwSm9obnMlMjBIb3BraW5zJTIwQVBMJTIwVGVjaG5pY2FsJTIwRGlnZXN0JTJDJTIwMTAlMkMlMjAyNjItMjY2LiZ1cmw9aHR0cHMlM0ElMkYlMkZ3d3cuamh1YXBsLmVkdSUyRlRlY2hEaWdlc3QlMkZ2aWV3cyUyRnBkZnMlMkZWMTBfTjNfMTk4OSUyRlYxMF9OM18xOTg5X1NpZ2lsbGl0b19DbGFzcy5wZGYmbHI9MjEzJm1pbWU9cGRmJmwxMG49cnUmc2lnbj1mNDFkYTliNzI5NjgyMjBlYjc1M2JkZjJjMTJiMmUwZCZrZXlubz0wIn0%3D&page=1&lang=en) авторов и опишите суть работы в нескольких абзацах текста.
    
