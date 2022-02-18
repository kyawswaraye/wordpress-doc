# August Host သင်ရိုးညွန်း

- [About Us](https://www.augusthost.com/about)

# Table of contents

1. [Introduction](#introduction)
2. [What is website](#what-is-website)
3. [What is HTML](#what-is-html)
   1. [Create Your First HTML file](#create-your-first-html-file)
   2. [Meta](#meta)
   3. [href Attribute](#href-attribute)
   4. [Adding Media](#adding-media)
   5. [Text Basics](#text-basic)
   6. [Semantics and Organization](#semantics-and-organization)
   7. [HTML Form](#html-form)
   8. [How to create a Table](#how-to-create-a-table)
   9. [Emmet](#emmet)
4. [What is CSS](#what-is-css)

## Introduction

## What is Website

## What is HTML

HTML ဆိုတာ Hyper Text Markup Language ကိုအတိုကောက်ပြောတာဖြစ်တယ်။HTML က webpages များကို ဖန်တီးရန်အတွက် စံသတ်မှတ်ထားသော ဘာသာစကားဖြစ်တယ်။HTML မှာကအားလုံးကို elements နဲ့ဖွဲ့စည်းထားတယ်။ဘယ်လိုရေးထားတယ်ဆိုတာကို browser ကိုပြောပြထားတာဖြစ်တယ်။ဒီနေရာမှာ ခေါင်းစဉ် ရေးထားတယ်။ဒီမှာက စာပိုဒ် ၊ ဒီမှာက လင့် စသည်ဖြင့်ပြောပြတာဖြစ်တယ်။ဥပမာ-header,paragraph,etc...
နားလည်ရမှာက HTML ဆိုတာ content တွေကိုရေးတာဖြစ်ပြီး css ဆိုတာက style တွေကိုရေးတာဖြစ်တယ်။

### Create Your First HTML file

ဒီသင်ခန်းစာမှာတော့ website တစ်ခုလောက်ဆွဲရအောင်။ပထမဆုံး VS Code editor ကိုဖွင့်မယ်။Folder တစ်ခုဆောက်ပြီး index.html ဆိုတဲ့ file ဆောက်ပါ။
`<h1>Hello World!</h1>`
ကိုရေးကြည့်ပါ။

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Hello World</title>
  </head>

  <body>
    <h1>Hello World!</h1>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores molestias
      cum et? Laudantium culpa dicta deserunt iusto velit impedit ipsa?
    </p>
  </body>
</html>
```

### Meta

အပေါ်ကပုံထဲက `<meta>` ဆိုတာ HTML စာမျက်နှာထဲမှာ ထည့်သွင်းလိုက်သော data အချက်အလက်များဖြစ်တယ်။`<head></head>` အတွင်းမှာရေးရပြီး ထို data ကို browser ပေါ်တွင်ပြသမည်မဟုတ်သော်လဲ search engine များကထို data ကိုအသုံးပြုပြီးရှာဖွေကြပါသည်။ Mobile မှာ စာလုံးတွေ scale ကြီးစေပြီးအဆင်ပြေပြေမြင်အောင် အောက်က တစ်ကြောင်းကိုထည့်ရပါမယ်။

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

### href Attribute

href attribute ဆိုတာက စာမျက်နှာတစ်ခုနဲ့ တစ်ခုချိတ်ဆက်ဖို့အတွက်အသုံးပြုတယ်။

```html
<a href=""></a>
```

`<a>` tag က hyperlink ဖြစ်ပြီး href attribute က link ကိုသွားတဲ့စာမျက်နှာရဲ့ url ကိုသတ်မှတ်ပေးတာဖြစ်တယ်။အောက်ကနမူနာပုံမှာ home page နဲ့ about page ကိုကူးပြောင်းနိုင်တဲ့ဥပမာဖြစ်ပါတယ်။

index.html မှာ

```html
<a href="about.html">about</a>
<h1>This is home page.</h1>
```

about.html မှာ

```html
<a href="index.html">Home</a>
<h1>This is about page.</h1>
```

### Adding Media

images, videos, audios file တွေကို page မှာထည့်လို့ရတယ်။

Add Image File

```html
<h1>Image</h1>
<img src="https://picsum.photos/500/200" alt="picture-1" />
```

Add Audio File

```html
<h1>Audio</h1>
<audio controls>
  <source
    src="https://cdn.pixabay.com/download/audio/2021/10/26/audio_0c72f89df1.mp3"
    type="audio/mpeg"
  />
</audio>
```

Add Video File

```html
<h1>Video</h1>
<video controls>
  <source src="video.mp4" type="video/mp4" />
</video>
```

### Text Basic

**Heading**  
heading တွေက h1 ကနေ h6 အထိရှိတယ်။page တစ်ခုမှာ h1 ကတစ်ခုပဲရှိသင့်တယ်။

**Bold & Italic**  
စာလုံးကို highlight ပြချင်ရင်က b နဲ့ strong နဲ့ ၂ ခုရှိတယ်။
စာလုံးကို စောင်းစောင်းလေးနဲ့ပြချင်ရင်က em နဲ့ i ကိုသုံးတယ်။

```html
<b>The cat hate the dog.</b>
<strong>The cat hate the dog.</strong>
<em>The cat hate the dog.</em>
<i>The cat hate the dog.</i>
```

> <b>The cat hate the dog.</b>  
> <strong>The cat hate the dog.</strong>  
> <em>The cat hate the dog.</em>  
> <i>The cat hate the dog.</i>

paragraph တစ်ခုလုံးကိုတော့ strong တို့ em တို့နဲ့မလုပ်သင့်ဘူး။ဘာလို့ဆိုတော့ html က element တွေကိုပဲရေးတာ။အဲ့လိုလုပ်ချင်ရင်က css နဲ့ရေးတာအကောင်းဆုံးပဲ။

**Bullet List**  
bullet list ဆိုတာက HTML element ထဲကနောက်ထပ် HTML element ဖြစ်တယ်။သူ့မှာ OrderList ရယ် UnorderList ဆိုပြီး ၂ ခုရှိတယ်။Menu ဆောက်တာတို့ List ပြတာတို့တွေမှာသုံးတယ်။

```html
<h1>OrderList</h1>
<ol>
  <li>Title One</li>
  <li>Title Two</li>
  <li>Title Three</li>
</ol>
<h1>UnorderList</h1>
<ul>
  <li>Title One</li>
  <li>Title Two</li>
  <li>Title Three</li>
</ul>
```

**Special Characters**  
 single quote, double quotes, ampersands, graterthan, lessthan, copyright, registered, treadmark ... ဒါတွေကိုက special character လို့ခေါ်တယ်။သူတို့ကိုရေးချင်ရင်က အောက်ကလိုမျိုးရေးတယ်။  
` &apos; &quot; &amp; &lt; &gt; &copy; &reg; &trade;`
output-

> &apos; &quot; &amp; &lt; &gt; &copy; &reg; &trade;

### Semantics and Organization

**strature**

```html
<header>
  <nav>
    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Contact</li>
    </ul>
  </nav>
</header>
<h1>My Website</h1>
<p>
  Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt voluptates
  pariatur id possimus, aliquam laudantium provident praesentium totam maiores
  similique?
</p>
<footer>
  <p>&copy; 2022-This is footer of the Website</p>
</footer>
```

**div**

`<div></div>` ဆိုတာက element တွေကို division အနေနဲ့ပိုင်းပြီး css ဒါမှမဟုတ် javasctipt နဲ့တွဲသုံးလို့ရအောင်လုပ်ထားတာပါ။ ဥပမာပြောရရင်-

```html
<div class="block-body"><p>Title</p></div>
<!-- block level elementဖြစ်တယ်။ -->
<span class="text-color">content</span>
<!-- inline element ဖြစ်တယ်။ -->
```

**comments**  
comment ကိုမိမိမှတ်ချင်သောနေရာများတွင်ရေးခဲ့လို့ရတယ်။browser က comment တွေ့ရင်ကျော်သွားတာကြောင့် developer ပဲမြင်နိုင်မှာဖြစ်တယ်။

```html
<!-- this is content start -->
<div>Title</div>
<!-- this is content end -->
```

### HTML Form

HTML form က user တွေထည့်သွင်းလိုက်တဲ့ အချက်အလက်များကို server သို့ပို့ပေးရန်အသုံးပြုတယ်။label မှာသုံးတဲ့ for က input ထဲက id နဲ့တူရမယ်။

```html
<form>
  <label for="name">Name</label>
  <input type="text" name="name" id="name" placeholder="name" />
  <label for="password">Password</label>
  <input type="password" name="password" id="password" placeholder="password" />
  <input type="submit" value="submit" />
</form>
```

**Different Types of input**

```html
<input type="button" />
<input type="checkbox" />
<input type="color" />
<input type="date" />
<input type="datetime-local" />
<input type="email" />
<input type="file" />
<input type="hidden" />
<input type="image" />
<input type="month" />
<input type="number" />
<input type="password" />
<input type="radio" />
<input type="range" />
<input type="reset" />
<input type="search" />
<input type="submit" />
<input type="tel" />
<input type="text" />
<input type="time" />
<input type="url" />
<input type="week" />
```

**Set of Option**

**Select**  
selected attribute က boolean ဖြစ်တယ်။

```html
<select name="favouriteColor" id="favouriteColor">
  <option value="colorRed">Red</option>
  <option value="colorGreen">Green</option>
  <option value="colorBlue">Blue</option>
</select>
```

**Radio**  
Radio က boolean ဖြစ်တယ်။

```html
<fieldset>
  <legend>What is Your Favourite Meal ?</legend>
  <input type="radio" name="favouriteMeal" id="breakfast" value="meal" />
  <label for="breakfast">Breakfast</label>
  <input type="radio" name="favouriteMeal" id="lunch" value="meal" />
  <label for="lunch">Lunch</label>
  <input type="radio" name="favouriteMeal" id="dinner" value="meal" />
  <label for="dinner">Dinner</label>
</fieldset>
```

**Checkbox**  
checkboxes တွေဟာ radio button နဲ့ပုံစံဆင်သော်လဲ radio မှာက တန်ဖိုးတစ်ခုပဲယူလို့ရပြီး checkboxes တွေမှာကတန်ဖိုးအားလုံးကိုယူလို့ရတယ်။

```html
<fieldset>
  <legend>What is Your Favourite Meal ?</legend>
  <input type="checkbox" name="favouriteMeal" id="breakfast" value="meal" />
  <label for="breakfast">Breakfast</label>
  <input type="checkbox" name="favouriteMeal" id="lunch" value="meal" />
  <label for="lunch">Lunch</label>
  <input type="checkbox" name="favouriteMeal" id="dinner" value="meal" />
  <label for="dinner">Dinner</label>
</fieldset>
```

### How to create a Table

table က row နဲ့ column နဲ့ဖွဲ့စည်းထားတဲ့ data အစုတစ်ခုဖြစ်တယ်။

```html
<table>
  <tr>
    <th>Name</th>
    <th>Phone no.</th>
    <th>Address</th>
  </tr>
  <tr>
    <td>John Doe</td>
    <td>01 234 567 89</td>
    <td>Lorem ipsum dolor sit amet.</td>
  </tr>
</table>
```

<table>
  <tr>
    <th>Name</th>
    <th>Phone no.</th>
    <th>Address</th>
  </tr>
  <tr>
    <td>John Doe</td>
    <td>01 234 567 89</td>
    <td>Lorem ipsum dolor sit amet.</td>
  </tr>
</table>

### Emmet

Emmet ဆိုတာ HTML tag တွေကို အတိုကောက်ရေးနည်းဖြစ်တယ်။ **_Html:5 (or) !_** ရေးပြီး tab ရိုက်လိုက်ရင်

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

**div#hello** ဆိုရင်

```html
<div id="hello"></div>
```

**div.hello** ဆိုရင်

```html
<div class="hello"></div>
```

**div\*3** ဆိုရင်

```html
<div></div>
<div></div>
<div></div>
```

**ul.mylist>li\*4** ဆိုရင်

```html
<ul class="mylist">
  <li></li>
  <li></li>
  <li></li>
  <li></li>
</ul>
```

## What is CSS

css ဆိုတာ Cascading Style Sheets ကိုအတိုကောက်ပြောတာဖြစ်တယ်။css က HTML elements တွေကို မည်သည့်ပုံစံ အဖြစ်ပြမည်ဆိုတာကို ကြည့်ကောင်းအောင်ရေးသားခြင်းဖြစ်ပါတယ်။တစ်ခုမှတ်ရမှာက css ကရေစီးနေသလိုပဲ။နောက်မှရေးတာကအလုပ်လုပ်ပါတယ်။

```html
<header>
  <h1 id="title">Title</h1>
  <p>Lorem ipsum dolor sit amet.</p>
  <p><span>Lorem ipsum dolor sit amet.</span></p>
</header>
<p class="highlight">Lorem ipsum dolor sit amet.</p>
<footer><p>This is footer</p></footer>
```

```css
h1 {
  color: red;
  text-align: center;
}
```

css ရေးရင် property နဲ့ value ကိုတွဲပြီးရေးတယ်။

### CSS Selector

Type Selector ဆိုတာက element နာမည်တွေကို select လုပ်တာ။ဥပမာ- **_p_** ဆိုရင် **_p_** အကုန်လုံးကို select လုပ်လိုက်တာပါ။

Descendent Selector ကတော့ `header p{color:green}` ဆိုပြီးတစ်ခုထဲကို select လုပ်ပါတယ်။ `header p span{color:red}` ဆိုပြီးစာလုံးတစ်လုံးချင်းစီကို ပြောင်းလို့ရပါတယ်။

HTML မှာဘယ်လိုပဲ format ချထားပါစေ ပြန်ပြင်လို့ရတယ်။  
`h1{font-size:200%; font-weight:bold;}`  
body ကအားလုံးရဲ့ parent ဖြစ်တယ်။`body{color:yellow;}` ဆိုပြီး `footer{color:red}` ဆိုရင် override လုပ်လို့ရပါတယ်။ဒါပေမယ့် `footer p{color:green}` ကအဆင့်အမြင့်ဆုံးပဲ။အတိအကျညွန်းထားလို့။ပြီးရင် class လာမယ်။ပြီး id လာမယ်။
