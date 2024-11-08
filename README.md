# Учебная Практика по Программированию

Добро пожаловать в репозиторий, посвящённый нашей учебной практике! В этом проекте мы реализуем несколько задач, включая составление модели бизнес-плана по разработке генератора паролей. Ниже приведена информация о каждом направлении работы, а также ссылки на соответствующие ветки.

## Содержание

- #### Модель Бизнес-Плана Формата IDEF0
- #### Программа: Генератор Паролей
- #### Листинг Кода
- #### Скриншоты Рабочей Программы

## Задача 1: Модель Бизнес-Плана Формата IDEF0

В данном разделе предоставлены наброски нашего бизнес-плана по разработке программы генератора паролей, выполненые при помощи компьютерных технологий:

## Контекстная диаграмма
![Контекстная диаграмма](https://github.com/meowqqhxd/ychebnaya/blob/main/%D0%9A%D0%BE%D0%BC%D0%BF%D0%BE%D0%B7%D0%B8%D1%86%D0%B8%D1%8F.jpg)

## Декомпозиция
![Декомпозиция](https://github.com/meowqqhxd/ychebnaya/blob/main/%D0%94%D0%B5%D0%BA%D0%BE%D0%BC%D0%BF%D0%BE%D0%B7%D0%B8%D1%86%D0%B8%D1%8F.jpg)





- **Описание проекта**: 
Нашей главной целью было создание программы для генерации паролей. Для начала нам необходимо было создать IDEF0, для наглядного показа нашего проекта, как более легкого и доступного способа донесения информации. 
Нами было создано две диаграммы: [контекстная диаграмма](https://github.com/meowqqhxd/ychebnaya/blob/main/%D0%9A%D0%BE%D0%BC%D0%BF%D0%BE%D0%B7%D0%B8%D1%86%D0%B8%D1%8F.jpg) и [декомпозиция.](https://github.com/meowqqhxd/ychebnaya/blob/main/%D0%94%D0%B5%D0%BA%D0%BE%D0%BC%D0%BF%D0%BE%D0%B7%D0%B8%D1%86%D0%B8%D1%8F.jpg)

## Контекстная диаграмма

 Для начала остановимся на контекстной, что она вообще из себя представляет. [Контекстная диаграмма](https://github.com/meowqqhxd/ychebnaya/blob/main/%D0%9A%D0%BE%D0%BC%D0%BF%D0%BE%D0%B7%D0%B8%D1%86%D0%B8%D1%8F.jpg) – это диаграмма, которая описывает систему на уровне «черного ящика», то есть только ее внешние свойства, не углубляясь внутрь программы. Нам необходимо было создать контекстную диаграмму для описания программы генерации паролей, поэтому очевидным становится то, что центром нашей диаграммы является блок с названием **«сгенерировать пароль»**. Далее остается только две основные вещи:
Данные, которые входят в блок (являются важными элементами для создания самой программы) и данные, которые мы получаем на выходе создания программы.

```1. Данные, которые входят в блок.```

Для написания данных элементов необходимо было учитывать, что нам может понадобится для создания программы для генерации паролей, поэтому нашу диаграмму будет удобнее читать начиная снизу справо-налево. Первым пунктом является «Алгоритм генерации», что безусловно важно для создания любого пароля. Второй пункт – UI. Довольно очевидный, но нужный пункт, так как в этой диаграмме мы описываем только внешние свойства нашей программы. Далее идет сложность, допустимые символы, минимальная и максимальная длина, что задает критерии для создания пароля для удобства пользования программой и ее практичности. После у нас остается два пункта **«Код проверки»** и **«Обновление алгоритмов генерации»**, что также упрощает пользование нашей программы и ее безопасность. 

```2. Данные, которые выходят из блока.```

Расписав все входные данные, можно приступать к выходным. На выходе мы получаем всего два пункта **«Сгенерированный пароль»**, что является основной целью нашей программы и **«Сообщение об успешной генерации»**.

## Декомпозиция

Для начала стоит разобраться что же такое «декомпозиция»?
[Декомпозиция](https://github.com/meowqqhxd/ychebnaya/blob/main/%D0%94%D0%B5%D0%BA%D0%BE%D0%BC%D0%BF%D0%BE%D0%B7%D0%B8%D1%86%D0%B8%D1%8F.jpg) – это процесс в программировании, предусмотренный для разбиение сложной системы или задачи, на более понятные и простые. Грубо говоря, сейчас мы углубляемся внутрь создания программы. 
Создав контекстную диаграмму, будет гораздо проще понимать, что конкретно нам предстоит сделать, поэтому для начала необходимо было выделить основные этапы. У нас их получилось четыре, давайте разберем.

```1.  Ввести условие генерации.```
Первый блок в нашей декомпозиции, являющийся начальным этапом создания программы. В нем умещается четыре подпункта: пользовательский ввод, обработка пользовательского ввода, UI и проверка корректности. Все они являются нужными для конкретного этого блока, поэтому на выходе мы получаем готовое «условие генерации» и переход к следующему блоку «сгенерировать пароль»

```2.  Сгенерировать пароль```
Второй блок в нашей декомпозиции, который уже нам знаком, включающий в себя три пункта: «проверка сложности и уникальности», «алгоритм генерации» и «генерация случайных символов». От этого блока в целом зависит дальнейшая судьба нашей программы, можно даже назвать его центром основной задачи. Поэтому на выходе мы получаем «сгенерированный пароль» (который проходит дальше через блок до «верифицировать пароль») и выход к блоку «вывести результат»

```3.  Вывести результат```
Третий блок в нашей декомпозиции, отвечающий за вывод результата с сгенерированным паролем, важная часть программы. Включает в себя три пункта: «Обработка ошибок», «Интерфейс с отображением» и «отображение пароля». Все они отвечают за вывод пароля, поэтому на выходе мы подходим к заключительному блоку «Верифицировать пароль».

```4.  Верифицировать пароль```
Последний четвертый блок в нашей декомпозиции, являющийся заключительным и отвечающим за верификацию пароля в нашей программе. Включает в себя всего два основных пункта: «Соответствие политике безопасности» и «Алгоритм проверки». А также перепрыгнув на блок через назад, включает в себя еще и «сгенерированный пароль», для его проверки. Тут в целом все это делается для того, чтобы пароль подходил под условия программы, поэтому на выходе мы получаем готовый «Проверенный пароль».

Проверенный пароль – является основной целью нашей программы по генерации паролей, это ключевой результат, прошедший через все проверки.

## Задача 2: **``Создание программы``**

И так, перейдём ближе к нашей программе, а точнее, к её сути. 

Программа, написанная на языке ``Visual Basic`` с использованием ``Windows Forms``.
Представляет собой набор компонентов визуального интерфейса (UI) для взаимодействия между пользователем, а также самим ПО.
Программа состоит из основной формы, на которой расположены следующие элементы управления:

#### **1) CheckBox**.
В нашем случае их четыре. Каждый отвечает за соответствующее действие. В первом случае пользователь может переключить положение данного элемента для того, чтобы генерировались заглавные буквы
Во втором случае, пользователь может переключить второй CheckBox для того, чтобы использовать только строчные буквы
В третьем случае можно использовать цифры в процессе генерации пароля, для этого необходимо переключить третий CheckBox
А также в заключении, пользователь может использовать специальные символы для генерации пароля.

#### **2) Button**.
В нашей приведённой программе содержится 2 кнопки:
Первая отвечает за генерацию пароля, т.е. пользователь выбирает подходящие варианты генерации, указывает длину пароля в следующем компоненте NumericUpDown, после этого используется кнопка “Сгенерировать пароль” для генерации пароля по заданным критериям.
Для облегчения взаимодействия пользователя и нашего ПО так же была добавлена кнопка “Копировать” (соответственно для того, чтобы скопировать сгенерированный пароль).

#### **3) NumericUpDown**.

В данном поле пользователь сам может указать длину пароля на тот, который ему нужен.
Также предусмотрены несколько вариантов ввода:
#### ```1.  ручной ввод```
#### ```2.  ползунки для увеличения или уменьшения заданного параметра.```

#### **4)  TextBox**
Данный компонент, можно сказать, что является самым важным в нашей программе. Именно он отвечает за вывод готового, сгенерированного пароля.
Пользователь может, либо сам скопировать сгенерированный пароль вручную, либо использовать, приведённую нами выше, кнопку “Копировать”

В целом, на этом визуальная составляющая интерфейса программы заканчивается. Как она выглядит можно посмотреть [Тут](https://github.com/meowqqhxd/ychebnaya/blob/%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BC%D0%BC%D0%BC-%D1%84%D0%BE%D1%82%D0%BE/%D0%A4%D0%BE%D1%80%D0%BC%D0%B0.png).

## Задача 3: **``Листинг кода``**

Самое главное в нашей программе – код, который отвечает за всё, что находится внутри программы. Перейдём к нему.

Для начала у нас есть объявление класса, в котором находятся несколько процедур.
Первая из них – объявление кнопки, а так же всех наших CheckBox

```go
Public Class Form1

    Private Sub BtnGenerate_Click(sender As Object, e As EventArgs) Handles BtnGenerate.Click
        Dim passwordLength As Integer = CInt(NumericUpDown1.Value)
        Dim useUpperCase As Boolean = CheckBoxUpperCase.Checked
        Dim useLowerCase As Boolean = CheckBoxLowerCase.Checked
        Dim useNumbers As Boolean = CheckBoxNumbers.Checked
        Dim useSpecialChars As Boolean = CheckBoxSpecialChars.Checked
```
Сразу после объявления расположена часть кода, отвечающая за предотвращение ошибок, т.е. если пользователь не выберет ни одной вариации конечного пароля, он получит уведомление о том, что необходимо выбрать хотя бы один параметр.

```go
        If Not (useUpperCase Or useLowerCase Or useNumbers Or useSpecialChars) Then
            MessageBox.Show("Выберите хотя бы один тип символа для генерации пароля.")
            Return
        End If
```
Следующим делом создаём функцию “Сгенерировать пароль” 
В данной функции указываем на положение переключателей CheckBox, а так же задаём перечень символов под определённый переключатель 

```go
    Private Function GeneratePassword(length As Integer, upper As Boolean, lower As Boolean, numbers As Boolean, special As Boolean) As String
        Dim allowedChars As New StringBuilder()

        If upper Then allowedChars.Append("ABCDEFGHIJKLMNOPQRSTUVWXYZ")
        If lower Then allowedChars.Append("abcdefghijklmnopqrstuvwxyz")
        If numbers Then allowedChars.Append("0123456789")
        If special Then allowedChars.Append("!@#$%^&*()-_=+[]{}|;:,.<>?")
```

В конечном итоге связываем кнопку “Копировать” с кодом и делаем её активной

```go
    Private Sub BtnCopy_Click(sender As Object, e As EventArgs) Handles BtnCopy.Click
        Clipboard.SetText(TextBoxPassword.Text)
        MessageBox.Show("Пароль скопирован в буфер обмена.")
    End Sub
```

Подробнее увидеть сам код можно [Здесь](https://github.com/meowqqhxd/ychebnaya/blob/%D0%BA%D0%BE%D0%B4%D0%B8%D0%BA-%D0%BB%D0%B8%D1%81%D1%82%D0%B8%D0%BA/Listing.txt)


## Задача 4: **``Фото работающей программы``**

Можно посмотреть в отдельной ветке [Тут](https://github.com/meowqqhxd/ychebnaya/blob/%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BC%D0%BC%D0%BC-%D1%84%D0%BE%D1%82%D0%BE/%D0%A0%D0%B0%D0%B1%D0%BE%D1%87%D0%B0%D1%8F_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0.jpg).

### Вывод

В ходе прохождения данной практикой были получены навыки построения моделей IDEF0 в двух видах:

```1) A0```

```2) A1```

Также за период прохождения практики была создана собственная программа по генерации паролей на языке программирования ```Visual Basic``` с использованием **Windows Forms** 
Наглядное представление программы позволило лучше понять её задачу, а также написать код для дальнейшего использования ПО.

За период прохождения практики были получены навыка вледния таким ресурсом, как Git и GitHub, что позволило загружать собственные проекты.
