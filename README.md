# CPS-researcher-test  <img src="https://ain17002254.files.wordpress.com/2017/09/3923-researchanddevelopmentbanner.jpg?w=150" />

Тестовое задание для кандидатов на должность CPS resercher.
- Пункты заданий расположены в порядке возрастания сложности. Выполнять можно любое понравившееся задание, столько пунктов, сколько сможете/захотите.
- Предпочтительно решать задачи, используя Python3 (и любой фреймворк для работы с нейросетями).
- Рассуждения по решению аналитических заданий можно оформить от руки, но желательно представить результаты в PDF с оформленным выводом (LaTeX или MathType).
- Каждое задание относится к тому или иному разделу машинного обучения или математического моделирования. Помимо решения задачи необходимо рассмотреть какую-либо статью, вышедшую в последние полгода на тему, связанную с заданием, и предложить как можно было бы использовать результаты этой статьи для решения данной задачи или анологичных данной.

## 1. Задание с теоретико-математическим смещением. (Оптимизация)

Заданы две функции:

<a href="https://www.codecogs.com/eqnedit.php?latex=$$&space;f_1(x,y)=\frac{1}{2}-\frac{\sin^2(\sqrt{x^2&plus;y^2})-\frac{1}{2}}{1&plus;\frac{x^2&plus;y^2}{1000}}&space;,&space;x,y&space;\in&space;\mathbb{R}$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$&space;f_1(x,y)=\frac{1}{2}-\frac{\sin^2(\sqrt{x^2&plus;y^2})-\frac{1}{2}}{1&plus;\frac{x^2&plus;y^2}{1000}}&space;,&space;x,y&space;\in&space;\mathbb{R}$$" title="$$ f_1(x,y)=\frac{1}{2}-\frac{\sin^2(\sqrt{x^2+y^2})-\frac{1}{2}}{1+\frac{x^2+y^2}{1000}} , x,y \in \mathbb{R}$$" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=$$f_2(z)=\frac{1}{1&plus;|z^6-1|}&space;,&space;z&space;\in&space;\mathbb{C},z=x&plus;iy&space;$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$f_2(z)=\frac{1}{1&plus;|z^6-1|}&space;,&space;z&space;\in&space;\mathbb{C},z=x&plus;iy&space;$$" title="$$f_2(z)=\frac{1}{1+|z^6-1|} , z \in \mathbb{C},z=x+iy $$" /></a>

- Найти аналитически глобальные максимумы этих функций.
- Построить графики этих функций.
- Представив, что функции являются исследуемым объектом, без аналитической формы задания (чёрный ящик), найти максимумы функций с помощью какого-либо численного метода. (Метод не обязательно нужно писать самому, можно использовать библиотечный).
- Для второй функции найти кратчайший путь по поверхности функции из одного максимума в любой другой аналитически или численно.

## 2. Задание с теоретико-математическим смещением. (Теория игр. Обучение с подкреплением. Моделирование.)

Задана следующая ситуация:
В центре круглого плоского бассейна плавает ученик. Внезапно к бассейну подошёл учитель. Учитель не умеет плавать, но бегает в 4 раза быстрее, чем ученик плавает. Ученик бегает быстрее в 4 раза когда находится на земле. В начальный момент времени ученик находится в центре бассейна. Учитель хочет поймать ученика и для этого выбирает следующую стратегию: если ученик на замле, то учитель бежит по направлению к нему, если ученик в воде, то учитель бегает по краю бассейна, бежит учитель по наименьшей дуге к точке радиальной проекции на край бассейна текущего положения ученика.
- Если существует выигрышная стратегия для ученика, найти её аналитически, если нет, доказать что её не существует.
- Визуализировать стратегию поведения используя простейшие примитивы.
- Решить задачу для случая неплоского бассейна.
- Запрограммировать ситуацию описанную в задаче так, чтобы ученик стал обучаемым объектом и каким либо способом обучить его. 

## 3. Задание с математико-инженерным смещением. (Анализ сигналов. Машинное обучение. Моделирование.)

Рассматривается некоторый детерминированный объект, который может быть описан дифференциальным уравнением 4-го порядка:

<a href="https://www.codecogs.com/eqnedit.php?latex=$$x^{(4)}&plus;4x^{(3)}&plus;2x^{(2)}&plus;3x^{(1)}&plus;kx^{(0)}=g&space;$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$x^{(4)}&plus;4x^{(3)}&plus;2x^{(2)}&plus;3x^{(1)}&plus;kx^{(0)}=g&space;$$" title="$$x^{(4)}+4x^{(3)}+2x^{(2)}+3x^{(1)}+kx^{(0)}=g $$" /></a>

относительно некоторой функции времени x(t) и произвольного ограниченного входного сигнала g(t). В скобочках у неизвестной функции указан порядок дифференцирования.

 <a href="https://www.codecogs.com/eqnedit.php?latex=$$k=\hat{f}(2.1)&space;$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$k=\hat{f}(2.1)&space;$$" title="$$k=\hat{f}(2.1) $$" /></a>
 
где <a href="https://www.codecogs.com/eqnedit.php?latex=$$&space;\hat{f}&space;$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$&space;\hat{f}&space;$$" title="$$ \hat{f} $$" /></a>  - непрерывная функция, которую требуется восстановить используя предоставленный набор данных `Regression_Test.json`.

- Восстановить коэффициент k и выяснить каким либо способом что происходит с системой спустя длительное время (устойчива ли система, неустойчива или стремиться к асимптотически фиксированному состоянию) если она стартует из состояния покоя (координата и все производные до 3 порядка включительно равны нулю).
- Промоделировать систему для разных воздействий g и построить графики "Воздействие - Отклик" <a href="https://www.codecogs.com/eqnedit.php?latex=$(x(t),g(t),t)$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$(x(t),g(t),t)$" title="$(x(t),g(t),t)$" /></a>.
- Восстановление закона <a href="https://www.codecogs.com/eqnedit.php?latex=$$&space;\hat{f}(x)&space;$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$&space;\hat{f}(x)&space;$$" title="$$ \hat{f}(x) $$" /></a> произвести с использование нейронной сети.

## 4. Задание на машинное обучение и программирование. (Порождающие модели. Машинное обучение.)

- Написать генератор изображений простых геометрических фигур (круг, квадрат, треугольник), который может генерировать разнообразные пиксельные ч.б. изображение фигур.
- Генератор должен использовать нейросети.
- С помощью полученного генератора написать программу, которая на вход принимает текст на русском языке, а на выходе генерирует фигуру: круг, если в тексте было больше букв "о" чем отсальных, треугольник, если больше букв "д", квадрат в ином случае.

Для облегчения работы с данными, вместо порождения фигур можно использовать порождение арабских цифр (для чего например можно использовать датасет MNIST) и порождать в третьем пунке цифру, которая больше всего раз попалась в тексте.

## 5. Задание на машинное обучение. (Классификация. Машинное обучение.)

Задан датасэт `ionosphere.arff` в котором находится описание и происхождение данных, а так же результаты авторов датасэта.
- Необходимо построить бинарный классификатор, качество которого не уступало бы качеству классификатора, полученного авторами (информация и ссылки содержатся внутря датасэта).
- Проанализируйте оригинальную [статью](https://docviewer.yandex.ru/view/403167255/?*=4j5bhtTV6gkTf03Ydarcmn9PiNh7InVybCI6Imh0dHBzOi8vd3d3LmpodWFwbC5lZHUvVGVjaERpZ2VzdC92aWV3cy9wZGZzL1YxMF9OM18xOTg5L1YxMF9OM18xOTg5X1NpZ2lsbGl0b19DbGFzcy5wZGYiLCJ0aXRsZSI6IlYxMF9OM18xOTg5X1NpZ2lsbGl0b19DbGFzcy5wZGYiLCJ1aWQiOiI0MDMxNjcyNTUiLCJ5dSI6IjkyODIzMDM1MTE1MzUxMjE3ODUiLCJub2lmcmFtZSI6dHJ1ZSwidHMiOjE1NDM0MjEzODY2OTAsInNlcnBQYXJhbXMiOiJsYW5nPWVuJm5hbWU9VjEwX04zXzE5ODlfU2lnaWxsaXRvX0NsYXNzLnBkZiZ0bT0xNTQzNDIxMzc3JnRsZD1ydSZ0ZXh0PVNpZ2lsbGl0byUyQyUyMFYuJTIwRy4lMkMlMjBXaW5nJTJDJTIwUy4lMjBQLiUyQyUyMEh1dHRvbiUyQyUyMEwuJTIwVi4lMkMlMjAlNUMlMjYlMjBCYWtlciUyQyUyMEsuJTIwQi4lMjAlMjgxOTg5JTI5LiUyMENsYXNzaWZpY2F0aW9uJTIwb2YlMjByYWRhciUyMHJldHVybnMlMjBmcm9tJTIwdGhlJTIwaW9ub3NwaGVyZSUyMHVzaW5nJTIwbmV1cmFsJTIwbmV0d29ya3MuJTIwSm9obnMlMjBIb3BraW5zJTIwQVBMJTIwVGVjaG5pY2FsJTIwRGlnZXN0JTJDJTIwMTAlMkMlMjAyNjItMjY2LiZ1cmw9aHR0cHMlM0ElMkYlMkZ3d3cuamh1YXBsLmVkdSUyRlRlY2hEaWdlc3QlMkZ2aWV3cyUyRnBkZnMlMkZWMTBfTjNfMTk4OSUyRlYxMF9OM18xOTg5X1NpZ2lsbGl0b19DbGFzcy5wZGYmbHI9MjEzJm1pbWU9cGRmJmwxMG49cnUmc2lnbj1mNDFkYTliNzI5NjgyMjBlYjc1M2JkZjJjMTJiMmUwZCZrZXlubz0wIn0%3D&page=1&lang=en) авторов и опишите суть работы в нескольких абзацах текста.
    
