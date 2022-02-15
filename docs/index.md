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
   6. [semantics and organization](#semantics-and-organization)

### Introduction

### What is Website

### What is HTML

HTML ဆိုတာ Hyper Text Markup Language ကိုအတိုကောက်ပြောတာဖြစ်တယ်။HTML က webpages များကို ဖန်တီးရန်အတွက် စံသတ်မှတ်ထားသော ဘာသာစကားဖြစ်တယ်။HTML မှာကအားလုံးကို elements နဲ့ဖွဲ့စည်းထားတယ်။ဘယ်လိုရေးထားတယ်ဆိုတာကို browser ကိုပြောပြထားတာဖြစ်တယ်။ဒီနေရာမှာ ခေါင်းစဉ် ရေးထားတယ်။ဒီမှာက စာပိုဒ် ၊ ဒီမှာက လင့် စသည်ဖြင့်ပြောပြတာဖြစ်တယ်။ဥပမာ-header,paragraph,etc...
နားလည်ရမှာက HTML ဆိုတာ content တွေကိုရေးတာဖြစ်ပြီး css ဆိုတာက style တွေကိုရေးတာဖြစ်တယ်။

### Create Your First HTML file

ဒီသင်ခန်းစာမှာတော့ website တစ်ခုလောက်ဆွဲရအောင်။ပထမဆုံး VS Code editor ကိုဖွင့်မယ်။Folder တစ်ခုဆောက်ပြီး index.html ဆိုတဲ့ file ဆောက်ပါ။
`<h1>Hello World!</h1>`
ကိုရေးကြည့်ပါ။

```
      <!DOCTYPE html>
      <html lang="en">

      <head>
         <meta charset="UTF-8">
         <meta http-equiv="X-UA-Compatible" content="IE=edge">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <title>Hello World</title>
      </head>

      <body>
         <h1>Hello World!</h1>
         <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores molestias
            cum et? Laudantium culpa dicta deserunt iusto velit impedit ipsa?</p>
      </body>

      </html>
```

### Meta

အပေါ်ကပုံထဲက `<meta>` ဆိုတာ HTML စာမျက်နှာထဲမှာ ထည့်သွင်းလိုက်သော data အချက်အလက်များဖြစ်တယ်။`<head></head>` အတွင်းမှာရေးရပြီး ထို data ကို browser ပေါ်တွင်ပြသမည်မဟုတ်သော်လဲ search engine များကထို data ကိုအသုံးပြုပြီးရှာဖွေကြပါသည်။

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
  <source src="music.mp3" type="audio/mpeg" />
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
output

> &apos; &quot; &amp; &lt; &gt; &copy; &reg; &trade;
