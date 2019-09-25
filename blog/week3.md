# Week 3 - Media Queries
Many people use a pocket-sized mobile device for many purposes.  Some of the purposes are reading, shopping, navigating, listening music, watching movies etc. These pocket sized devices come in different sizes. Many cellphone and tablet manufacturing companies have different sizes for the same products. Imagine if a developer had to develop web-sites for each device!! Luckily, developers are smart hipisters as we all know, so they have a solution for every problem. The solution is called a responsive website design which changes sizes as it fits, and the content adjusts to the screen size. How is it done? the answer is called ## Media Queries. Media Queries help a website to be responsive. That means that any text, images, forms and etc that are incorporated into a websites for the use of larger screens such as desktops, can be seen in the same way on the pocket-sized screens, such as tablets and cellphones.
If we have a code:
```
 Body 
{ 
Background-color: white;
}

.container {
Margin: 0 auto;
Width: 95%;
max-width: 850px;
}

H1 
{
Color: #cc4425;
Font-family: ‘Oswalds’, sans-serif;
Font-size: 3rem;
font-weight: 700;
Margin: 0rem 0rem 0.5rem 0rem;
Text-transformation: uppercase;
}

H1 span {
Color: #DDD;;
Font-size: 0.5rem;
Display: block;
}

 p {
Color: #3E4147;
font-family: ‘Arvo’, serif;
Font-size: 1rem;
font-weight: 400;
Light-hight: 1.75;
Margin: 0rem 0rem 2rem 0rem;
}
```
and followed by:
```
@media ( rule) {font: x;
}

@media ( min-wid: 600px) 
 p { font-size : 1.25rem;
}

@media ( min-wid: 800px) 
 p { 
font-size : 1.5rem;
Line-height: 1.5;
}
```

-With CSS The last rule wins; so the media queries overrides the "p" properties stated above 


If we design the page for mobile screen and will get bigger on a desk-top
We should use:
```
@media ( min-width: 600px)
{ 
}
```
The other way around:
```
@media ( max-width: 600px)
{ 
}
```
Another way to design it would be by focusing on orientation instead of on Mx-width or min-width
```
@media ( orientation: landscape )
{
}
@media ( orientation: portraite)
{
}
```
There are other properties as well.
