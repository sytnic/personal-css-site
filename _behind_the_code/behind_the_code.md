# Linkedin CSS Essential Training 08-2023

CSS Essential Training (2023)  
https://codepen.io/collection/YyadbL

## Links

CSS Essential Training (2023)
https://codepen.io/collection/YyadbL
https://codepen.io/collection/YyadbL

Lorem ipsum   
https://meettheipsums.com/

Photos  
https://unsplash.com/  

Icons  
https://www.iconfinder.com/

https://www.freepik.com/

Изменять размер изображений  
https://www.adobe.com/express/  
https://www.shutterstock.com/  

W3C - Functional Images  
https://www.w3.org/WAI/tutorials/images/functional/

W3C - CSS
https://www.w3.org/Style/CSS/
https://www.w3.org/Style/CSS/Overview.ru.html

https://www.w3.org/Style/CSS/current-work

## 018-The color property and values

Имена цветов

https://developer.mozilla.org/en-US/docs/Web/CSS/named-color

Цвета по группам

https://colours.neilorangepeel.com/

Шестнадцетиричная прозрачность

https://davidwalsh.name/hex-opacity

Как вычислять шестнадцетиричные значения

https://www.wikihow.com/Understand-Hexadecimal

Все типы создания цветов

https://developer.mozilla.org/en-US/docs/Web/CSS/color_value

## 019-Creating a color palette

Выбор набора цветов

https://coolors.co/ -  
Надо нажать кнопку "Start the Generator" и перебирать набор цветов нажатием пробела. Понравившиеся цвета можно отметить неизменными, нажав знак замочка.  

## 026-Project Adding background styles

https://www.webfx.com/web-design/hex-to-rgb/

## 027-Pseudo classes and pseudo elements

02_13 Pseudo-classes and pseudo-elements  
https://codepen.io/christinatruong/pen/jOeyPPR

https://developer.mozilla.org/en-US/docs/Web/CSS/:active

## 029-Specificity

Пример высчитывания специфичности

<img src="img/specify_calc.jpg" alt="drawing" width="600"/>

## 032-The box model properties

<img src="img/short_padding.jpg" alt="drawing" width="600"/>

https://developer.mozilla.org/en-US/docs/Web/CSS/border-width

<img src="img/short_border.jpg" alt="drawing" width="600"/>

## 033-Box sizing and the box model fix

Разница в вычислении размера контента:

<img src="img/box-sizing.jpg" alt="drawing" width="600"/>

03_03 Box-sizing  
https://codepen.io/christinatruong/pen/bGxvOeG

`border-box` не изменяет размеры элементов, в отличие от `content-box`.  

Исправление коробочной модели:  

```css
    /*
    https://www.paulirish.com/2012/box-sizing-border-box-ftw/
    */

    html {
    box-sizing: border-box;
    }

    *, *:before, *:after {
    box-sizing: inherit;
    }
```

## 034-Inline block and display

03_04 Inline, block and display  
https://codepen.io/christinatruong/pen/xxaYNLK

## 036-Debugging with developer tools

Рекомендуемый курс:

> Workflow Tools for Web Developers

## 037-Managing box model quirks

03_07 Box model quirks   
https://codepen.io/christinatruong/pen/QWVmjZW

## 044-Layouts with the float property

04_02 Floats

https://codepen.io/christinatruong/pen/JjaZJeK

## 045-Clearing floats

В плавающих элементах часто получалось, что контент выходил за пределы отведённого размера элемента. Чтобы избежать этого есть несколько способов.  

Первый способ: overflow 

overflow: hidden; - скрывает часть контента, который вышел за пределы элемента.  
overflow: auto; - появляется полоса прокрутки, когда контент вышел за пределы элемента.

```html
    <div class="parent">
        <div class="floated">floated element</div>
        <div class="floated">floated element</div>
    </div>

    .floated {
        float: left;
    }

    .parent {
        overflow: hidden;
        /* OR */
        overflow: auto;
    }

```

Способ Clearfix Hack. Устарел. В основном требовался из-за Internet Explorer.

Самый современный способ: display. Заставляет контент полностью входить в контейнер, не выходя за его пределы. Видимо, повторяет поведение flex и grid.  

```html
    .parent {
        display: flow-root;
    }

    <div class="parent">
        <p>floated element</p>
        <p>floated element</p>
    </div>

```

##