1. [Последовательность событий при проведении документа](#последовательность-событий-при-проведении-документа)
2. [Последовательность событий при отмене проведения](#последовательность-событий-при-отмене-проведения)
3. [Последовательность событий при открытии формы](#последовательность-событий-при-открытии-формы)
4. [ПодпискиНаСобытияОбъектовМетаданных.epf](#подпискинасобытияобъектовметаданныхepf)

## Последовательность событий при проведении документа:
![alt text](https://github.com/kuzyara/Sequences-of-events-for-1C-objects/blob/master/ПоследовательностьСобытийДокумента_v1.1.png?raw=true)

**Про подписки:**
* Дополнение1: все подписки на события выполняются после стандартных обработчиков Объекта(не формы) и выполняются тоже только на сервере
* Дополнение2:  подписки на события для одинаковых источников и действий выполняются в порядке размещения подписок в конфигураторе сверзу вниз (т.е. в таком же порядке, как и в дереве метаданных)
* Дополнение3: подписки с источником общего типа ДокументОбъект, СправочникОбъект выполняются позже, чем с источником  конкретного типа, даже если он составной.

## Последовательность событий при отмене проведения:
![alt text](https://github.com/kuzyara/Sequences-of-events-for-1C-objects/blob/master/ПоследовательностьСобытийДокументаОтменаПроведения_v1.1.png)

## Последовательность событий при открытии формы:
![alt text](https://github.com/kuzyara/Sequences-of-events-for-1C-objects/blob/master/FormSeqDiagram.png)

Источники: 
* http://1centerprise8.blogspot.com/2015/03/posled-sobytij-document.html
* http://1centerprise8.blogspot.com/2016/08/sobytija-formy-obekta.html
* https://infostart.ru/public/1098803/

## ПодпискиНаСобытияОбъектовМетаданных.epf
* ОФ и УФ __[Скачать](https://github.com/kuzyara/Sequences-of-events-for-1C-objects/releases/latest/download/Sequences-of-events-for-1C-objects.zip)__ ![GitHub All Releases](https://img.shields.io/github/downloads/kuzyara/Sequences-of-events-for-1C-objects/total?style=flat-square)
* разделение по документам, справочникам, регистрам и т.д.
* соблюдается подрядок вызова как в дереве метаданных
![image](https://user-images.githubusercontent.com/2604430/63091901-1e85fb80-bf8a-11e9-863f-e096ddc6bb99.png)
