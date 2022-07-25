# CSS

Done: Yes

## first project

```css
<!--
; => two explan you end the first property . 
## if you want link class write
.class name 
## if you want link id write
#id name 
-->
selector{
property one : ; 
property two : ; 
}
```

## Edit on link

```css
/* 
text-decoration: ; بتقدر من خلالها تعدل علي الخط الازرق الي تحت اللينك 
none : لو عايز الخط يتشال من تحت اللينك 
overline: لو الخط يكون فوق الكلام 
line-throought : لو عايز الخط يكون جوه الكلام 
cursor : تتحكم في شكل الماوس لما يقف علي اللينك 
a:hover{
	color: red ; 
} : لون اللينك لما تيجي تدوس عليه 

*/ 
```

## Display

```css
/*
# متقدرش تتحكم في طول و عرض العناصر الاين لاين و لكن تقدر تتحكم في طول و عرض العناصر البلوك 
display : عشان تحول العناصر البلوك لاين لاين و العكس 
#inline-block : ده عشان تعمله اين لاين و يتنفز عليه خصائص البلوك 
#none : عشان اخفي  عنصر معين من الموقع 
visibility : عشان اخفي العنصر بس مفيش يبقي مكانه فاضي 
#hidden:   الامر المستخدم لاخفاء العنصر 

*/
```

## overflow

```css
/*
overflow : عشان لو المحتوي الي انت كاتبه اكبر من الديف 
#hidden : عشان اقله لو المحتوي اكبر من الديف ميظهروش 
#scroll : عشان يقدر يعمل سكرول 
#auto : ده احسنهم عشان هو بيظبط ال الكلام 
*/
```

## List

```css
ul {
	list-style-type: ; 
	/*
	disc : دائرة مقفولة 
	circle : دائرة مفتوحة 
	square : مربع 
	decimal : لو عايز ارقمها 
	none : لو تشيل الاشكال خالص */
	list-style-position : ; 
	/*
	inside : لو عايز الاشكال تكون داخله معاك في الاطار 
	
	*/
	list-style-image: url("") ;
	/*
	لو عايز تخلي الشكل صورة */
	list-style: ; 
	/*
	ممكن تحط الي انت عايزه */
}
```

## Float

```css
/*
float : بتتحكم في البوشن بتاع الكلام بس بطلعه بره نطاق العمل 
يعني لو انت كتبت حاجه و راها هتيجي جنبها عادي من غير اي فاصل 
clear : عشان احل مشكلة الفلوت 
.clear { 
					clear : both ;  }
*/ 
```

## position

```css
	fixed : الكلام بيطلع و بينزل معايا 
	relative :  الكلام مرتبط  باول قيمة ليه  و مكانه لسه محجوز 
	absolute:  الكلام مرتبط بالاب بتاعه و خارج اطار العمل و فوق كل العناصر 
	sticky : نفس عمل الفيكسد 
```

## pseudo

```css
pseudo classes {a:visited {
	 color: red ; 
/*
لما ازور الموقع يجبلي لون معين 
*/}
.check:checked{
	opacity : ; // الشفافية 
// 0 small opacity 
// 1 large opacity 
}
.text:focus{
outline:none; 
} }
Example : 
// <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
pseudo element {
p::first-letter {
	color : red  ; }
p::first-line{
 font-family :arial  ; }

} 
#selection : لون خلفية الكلام لما اظلل عليه 
::selection {
background : red ; 
color: white ; 

}
// لو عايز السيليكشن يحصل في الموقع كله 
```

## Add content

```css
// to add text after or before text ; 
selector:: after {
content: "test" ; 
//و الكلمة دي هتتضاف في نهاية كل كلام 

}
```

## @media

```css
#التوافقية علي كل الاجهزه 
@media screen and (min-width: px ) (max-width: px ) 
```

## justify hr or vr

```css
/*    Horzental

	dispaly: flex; 
	justify-content: center; 
	flex-direction: row; 
	or 
	flex-direction : coloum ; 
_____________________________
flex-wrap: wrap; 
عشان لو الكورت كتيره متصغرش 

    */
/*  vertical 

item-align: center ; 

*/
```

## box-shadow

```css
/*
box-shadow : (top && bottom ) (+ right) or (- left) (blur الشفافية ) rgb(red green blue / focus  التركيز )  

*/
```