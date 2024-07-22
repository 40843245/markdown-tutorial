# markdown tutorial
## Text
### Heading 
There are six different types of headings, from heading 1 to heading 6. 

Heading 1 has the biggest text among these headings. 

While heading 6 has the smallest text among these headings.

| Markdown	| HTML | Rendered Output |
| --------- | ---- | --------------- |
| # Heading level 1 | `<h1>Heading level 1</h1>` |	<h1>Heading level 1</h1> | 
| ## Heading level 2	| `<h2>Heading level 2</h2>` | <h2>Heading level 2</h2>	| 
| ### Heading level 3	| `<h3>Heading level 3</h3>` | <h3>Heading level 3</h3>	| 
| #### Heading level 4	| `<h4>Heading level 4</h4>` | <h4>Heading level 4</h4> |
| ##### Heading level 5	| `<h5>Heading level 5</h5>` | <h5>Heading level 5</h5> |
| ###### Heading level 6 | `<h6>Heading level 6</h6>`	| <h6>Heading level 6</h6> |

#### Alternative Syntax

| Markdown | HTML | Rendered Output |
| -------- | ---- | --------------- |
| Heading level 1 <br> ===============	| `<h1>Heading level 1</h1>` | <h1>Heading level 1</h1> |
| Heading level 2 <br> ---------------	| `<h2>Heading level 2</h2>` | <h2>Heading level 2</h2> |

#### **NOTES**
+ Don't forget to put one space between `#` and the first word.
+ `#` must be consecutive. For example, `## Heading 2` and `# # Heading 2` are **NOT** equivalent.

### Paragraphs
To create paragraphs, use a blank line to separate one or more lines of text.

| Markdown | HTML | Rendered Output |
| -------- | ---- | --------------- |
| I really like using Markdown. <br> <br> I think I'll use it to format all of my documents from now on.	| `<p>I really like using Markdown.</p> <p>I think I'll use it to format all of my documents from now on.</p>` | <p>I really like using Markdown.</p> <p>I think I'll use it to format all of my documents from now on.</p>
  
#### **NOTES**
Unless the paragraph is in a list, don’t indent paragraphs with spaces or tabs.

### Line Breaks
To create a line break or new line (in html `<br>`), end a line with two or more spaces, and then type return.

| Markdown | HTML | Rendered Output |
| -------- | ---- | --------------- |
| This is the first line.  <br> And this is the second line. |	`<p>This is the first line.<br> And this is the second line.</p>`	 | <p>This is the first line.<br> And this is the second line.</p> |

#### **NOTES**
Unlike C, one can ***NOT*** `\` to break a new line.

See the example on [Line Break Best Practices](https://www.markdownguide.org/basic-syntax/#line-break-best-practices)

## Emphasis of text
### Bold

| Markdown | HTML | Rendered Output |
| -------- | ----- | -------------- |
| `I just love **bold text**`. |	`I just love <strong>bold text</strong>`.	| I just love <strong>bold text</strong> |
| `I just love __bold text__.` | `I just love <strong>bold text</strong>.` | I just love <strong>bold text</strong>. |
| `Love**is**bold`	| `Love<strong>is</strong>` | Love**is**bold |

#### **NOTES**
There don't exist this syntax. Such as `Love__is__bold`.

### Italic

| Markdown | HTML | Rendered Output |
| -------- | ---- | --------------- |
| `Italicized text is the *cat's meow*.` | `Italicized text is the <em>cat's meow</em>.`	| Italicized text is the <em>cat's meow</em>. |
| `Italicized text is the _cat's meow_.`	| `Italicized text is the <em>cat's meow</em>.`	| Italicized text is the <em>cat's meow</em>. | 
| `A*cat*meow` | `A<em>cat</em>meow` | A*cat*meow

#### **NOTES**
There don't exist this syntax. Such as `A_cat_meow`.

### Bold and Italic

| Markdown | HTML |	Rendered Output |
| -------- | ---- | --------------- |
| `This text is ***really important***.` | `This text is <em><strong>really important</strong></em>.` | This text is <em><strong>really important</strong></em>.|
| `This text is ___really important___.` | `This text is <em><strong>really important</strong></em>.` |	This text is <em><strong>really important</strong></em> |
| `This text is __*really important*__.`	| `This text is <em><strong>really important</strong></em>.`	| This text is <em><strong>really important</strong></em> |
| `This text is **_really important_**.` | `This text is <em><strong>really important</strong></em>.` | This text is <em><strong>really important</strong></em> |
| `This is really***very***important text.`	| `This is really<em><strong>very</strong></em>important text.`	| This text is <em><strong>really important</strong></em> |

#### **NOTES**
There don't exist this syntax. Such as `This is really___very__important text.`.

#### **NOTES** 
The order of the em and strong tags might be reversed depending on the Markdown processor you're using.

## Blockquotes
### Blockquotes with Single Line
To create a blockquote, add a > in front of a paragraph.

    > Dorothy followed her through many of the beautiful rooms in her castle.

The rendered output looks like this:

> Dorothy followed her through many of the beautiful rooms in her castle.

### Blockquotes with Multiple Paragraphs

Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
    
The rendered output looks like this:

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.


### Nested Blockquotes
Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.
    
    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

The rendered output looks like this:

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### Multiple Nested Blockquotes

Let's dig in with several examples.

+ Example 1: 3-level nested blcokquotes

    > I'm so excited. 
    > I didn't sleep well last night.
    >> We're going bird watching the camping.
    > It's a school assignment, 
    >>> so don't just play around. 
    > Please take it seriously.
    > We have to spend 3 weeks looking for birds.

The rendered output looks like this:

> I'm so excited. 
> I didn't sleep well last night.
>> We're going bird watching the camping.
> It's a school assignment, 
>>> so don't just play around. 
> Please take it seriously.
> We have to spend 3 weeks looking for birds.

+ Example 2: 12-level nested blockquotes

      > hey you young lady, can I have your seat?
      > why?
      >> why you say?
      > can you see this maternity badge here?
      >>> maternity badge?
      > it's a beige to prove that the holder of the beige is pregnant.
      >>>> yes as you can see I'm pregnant.
      > it's tiring to stand still for the baby.
      >>>>> give.
      > give up your seat.
      >>>>>> I know that pregnant women have a hard time
      > (O.S. but her tone can she be nicer )
      >>>>>>> but Midori is sitting
      > because she has a headache
      >>>>>>>>> hey dck she's still young a little pant
      > you would be a problem
      >>>>>>>>>> but it's a matter of life or death of my child
      > can you understand hold up now
      >>>>>>>>>>> you're too much are
      > Other poeple says: they arguing can't they do this elsewhere
      >>>>>>>>>>>> gosh thanks to this keys
      > I'm attracting so much attention

The rendered output looks like this:

> hey you young lady, can I have your seat?
> why?
>> why you say?
> can you see this maternity badge here?
>>> maternity badge?
> it's a beige to prove that the holder of the beige is pregnant.
>>>> yes as you can see I'm pregnant.
> it's tiring to stand still for the baby.
>>>>> give.
> give up your seat.
>>>>>> I know that pregnant women have a hard time
> (O.S. but her tone can she be nicer )
>>>>>>> but Midori is sitting
> because she has a headache
>>>>>>>>> hey dck she's still young a little pant
> you would be a problem
>>>>>>>>>> but it's a matter of life or death of my child
> can you understand hold up now
>>>>>>>>>>> you're too much are
> Other poeple says: they arguing can't they do this elsewhere
>>>>>>>>>>> gosh thanks to this keys
> I'm attracting so much attention

+ Example 3: 4-level blockquotes where there are no one `>` as seperator in each different level
  
      > I'm glad you finally understand.
      >> you're lucky. Midory is way too nice huh.
      >>> it's all for to say to an unwell person.
      >>>> it's not a big deal AE what she's got a point.

The rendered output looks like this:

> I'm glad you finally understand.
>> you're lucky. Midory is way too nice huh.
>>> it's all for to say to an unwell person.
>>>> it's not a big deal AE what she's got a point.

+ Example 4:

      > in the following week,
      >> ouch ouch are you okay?
      >>> stepping into the gap between the train and the platform...
      >>>> why are you always so careless?
      >>> I wasn't paying attention because the train was about to leave once we get over there
      >> we need to get it treat.
      > sorry to trouble you.

The rendered output looks like this:

> in the following week,
>> ouch ouch are you okay?
>>> stepping into the gap between the train and the platform...
>>>> why are you always so careless?
>>> I wasn't paying attention because the train was about to leave once we get over there
>> we need to get it treat.
> sorry to trouble you.


> we still have two more weeks left for bird watching,
> so you need to be more careful. huh those are the kids from last
week they're here again how dare they
embrace me last time hey you
guys stand up and give me your
seat but K is injured I'm sorry could
you ask someone else for the seat aari
just BR her ankle what prano do they
know each other unbelievable how can she
demand seed from an injured girl what uh
I'm fine come on please sit down Carrie
are you able to steal I'm okay I'm good
at standing on one foot the swaying

