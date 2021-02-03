## Yaroslav Yagodarov

## Contact Info
* **Mobile:** +7(912)8722088
* **e-mail1:** ya.yagodarov@gmail.com
* **e-mail2:** slava-ross@yandex.ru
* **telegram:** @yagodarov

## Summary
I dreamed of becoming a programmer for many years since I graduated from middle school. But I was not able to get a job as a programmer despite the fact that I studied as a system engineer later at university,
because my specialization, that was _"computer systems and networks"_.
I started amateur web development around 2004. It was a user accounting system, as a part of billing system for VoIP clients. It was based on HTML4, CSS2, PHP4 and PostgreSQL6.X.
Its interface had a terrible layout according to modern criteria and there was a misuse some of the above technologies. 
Later at another job, I've deployed a similar system for network equipment accounting. It was slightly more complex but also imperfect due to my lack of knowledge of modern web technologies.
So I started taking online web development courses and fate brought me to RS-School.

## Skills

I've got an entry level in following languages and technologies: HTML, CSS, JavaScript, PHP, MySQL, PostgreSQL, jQuery, Ajax, Python, Pascal and little experience in ANSI C, C++, x86, AVR, C51, Z80 assemblers that got during my hobbies.

## Code example
```javascript
$(document).ready( function() {

var v;
var reg = 0;
var dispReg = '0';
var operSign = '';
var operFlag = false;
var actFlag = false;
var equFlag = false;

function dispOut( targetID, stringOut ) {
    $(targetID).empty();
    $(targetID).html( '<span>' + stringOut + '</span>' );
}

function reset() {
    reg = 0;
    dispReg = '0';
    operSign = '';
    operFlag = false;
    actFlag = false;
    equFlag = false;
    dispOut( '#dispResult', dispReg );
    dispOut( '#dispOper', operSign );
}

reset();

$('#clr').click( function() {
    reset();
});

$('#equ').click( function() {
    reg = eval( Number( reg ) + operSign + Number( dispReg ) );
    dispOut( '#dispResult', reg );
    operFlag = false;
    actFlag = false;
    equFlag = true;
});

$('.numButton').click( function() {
    v=$(this).attr( 'value' );
    if ( operFlag ) {
	actFlag = true;
	dispReg = 0;
    }
    if ( equFlag ) {
	dispReg = 0;
    }
    operFlag = false;
    dispReg = dispReg * 10 + Number( v );
    equFlag = false;
    dispOut( '#dispResult', dispReg );
});

$('.signButton').click( function() {
    v=$(this).attr( 'value' );
    if ( !operFlag ) {
	if ( actFlag ) {
	    reg = eval( Number( reg ) + operSign + Number( dispReg ) );
	    dispOut( '#dispResult', reg );
	}
	else {
	    if ( !equFlag ) {
		reg = dispReg;
	    }
	}
	operFlag = true;
    }
    operSign = v;
    equFlag = false;
    dispOut( '#dispOper', operSign );
});
});
```

## Experience
* [HtmlAcademy - Progress](https://htmlacademy.ru/profile/id886151/progress)
* [CodeAcademy - Profile](https://www.codecademy.com/profiles/SlavaRoss)
* [Calculator - JavaScript](https://github.com/slava-ross/js-calc)
* [MVC web-application (Laravel PHP framework)](https://github.com/slava-ross/laravel_gtx/tree/ajax_crud)
* [MVC web-application with Ajax](https://github.com/slava-ross/news-mvc-user-mysql) 

## Education and qualifications
### 1997 – 2002 Izhevsk State Technical University, Computer Engineering

* Microprocessor technology
* System programming
* Data protection
* Computer Networks

Most of my coursework was focused on Electronics, Hardware Engineering, System Programming but I minored in Economics.

**I'm currently studying in:**
* [HtmlAcademy](https://htmlacademy.ru/profile/id886151/progress)
* [EPAM Java-online courses](https://www.training.ru/#!/Training/2355?lang=ru)
* [JavaBegin courses](https://javabegin.ru/courses)

## English language

* English lessons in school, college, university (_insignificant experience_).
* Readings: in everyday tasks at past and current work (docs reading, info searching on the Internet).
* I've got pre-intermediate skill in Language Center **"Lingua City"** ( at the present time: [**Cambridge-Center**](https://cambridge-center.ru) ) in the year of 2016.


