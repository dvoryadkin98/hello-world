##  Все началось с простого приложения SimUDuck

Джо  работает на компанию, выпустившую чрезвычайно успешный имитатор пруда. В этой игре представлен пруд, в котором плавают и крякают утки разных  видов. Проектировщики системы воспользовались стандартным приемом ООП и определели  суперкласс Duck, на основе которого объявляются типы конкретных видов уток.

![kartinka1](https://github.com/dvoryadkin98/hello-world/blob/master/images/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA.PNG?raw=true)

За последний год компания испытывала жесткое давление со стороны конкурентов. Через неделю долгих выездных совещаний за игрой в гольф руководство компании решило, чтио пришло время серьезных изменений. Нужно сделать что-то *действительно* впечатляющее, что можно было бы продемонстрировать на предстоящем собрании акционеров на *следующей неделе*.

## Теперь утки будут ЛЕТАТЬ

Начальство решило, что летающие утки - именно та "изюминка", которая сокрушит всех конкурентов. И конечно, начальство Джо пообещало, что Джо легко соорудит что-нибудь этакое в течение недели. "В конце концов, он ООП-программист... *Какие могут быть трудности?"*

![kartinka2](https://github.com/dvoryadkin98/hello-world/blob/master/images/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA1.PNG)

## Но тут ввсе пошло наперекосяк...

#Что произошло?

Джо не сообразил, что *летать* должны *не все* субклассы Duck. Новое поведение, добавленное в суперкласс Duck, оказалось *неподходящим* для некоторых субклассов. И теперь в программе начали летать неодушевленные объекты.

*Локальное изменение кода привело к нелокальному побочному эффекту (летающие резиновые утки!)*

![kartinka3](https://github.com/dvoryadkin98/hello-world/blob/master/images/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA2.PNG)

## Джо думает о наследовании...

![kartinka4](https://github.com/dvoryadkin98/hello-world/blob/master/images/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA4.PNG)
![kartinka5](https://github.com/dvoryadkin98/hello-world/blob/master/images/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA5.PNG)

## Как насчет интерфейса?

Джо понял, что наследование не решит проблему - он только что получил служебную записку, в которой говорится, что продукт должен обновлятьься каждые 6 месяцев (причем начальство еще не знает, как именно). Джо знает, что спецификация будет изменяться, а ему придется искать (и, возможно, переопределять) методы fly() и quack() для каждого нового субкласса, включаемого в программу... *вечно*.

Итак, ему нужен более простой способ заставить летать или крякать только *некоторых* (но не всех!) уток.

![kartinka5](https://github.com/dvoryadkin98/hello-world/blob/master/images/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA3.PNG)

## А что ВЫ думаете об этой архитектуре?
