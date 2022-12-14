# Markdown basics

## Userstory-001: How to make a codeblock

Below is just a simple written function, with a nice "framing" to it.
It doesn't do much, but it looks great.

```js
function Kristofer () {
   return Kristofer;
}
```

Just add "```"js and close it.

##  Userstory-002: How to make a java codeblock in markdown

Below is a simple function in java 
```
public class Main {
public static void main(String[] args)
System.out.println("Hello World")
}
```

## Userstory 003: How to insert an image in markdown

This is a quick guide on how to make images work in markdown. No fuzz, just how to put memes inside an .md file such as this one:

<img src="https://www.meme-arsenal.com/memes/4105d28f45566683f9800958847c4664.jpg" alt="mouth girl meme" style="float: left;" />

You can use standard HTML. Inline styling for CSS properties is allowed.


## View example below:

```HTML
<img src="<YOUR-DIRECT LINK>" alt="<IMAGE-DESC>" style="<YOUR-STYLE>" />
```

## Userstory-004: Making a javascript codeblock

```js
export default ({ products }) => {
    return products.map(product => {
        return (
            <div className="product" key={product.id}>
                <div className="p-name">{product.name}</div>
                <div className="p-desc">{product.description}</div>
            </div>
        );
    });
};
```

Just add "```"js and close it.

## Userstory-005: Brackets runt kommentar och parantes runt länk

[Bra musik!](https://www.youtube.com/watch?v=dQw4w9WgXcQ)

## Userstory-006: How to make tables in markdown
Sträck för att göra table -- för kolumn


| J | O | N | T | E |
|---|---|---|---|---|
| M | A | R | K | U |
| E | L | I | A | Z |
|   |   |   |   |   |

## Userstory-007: How to make bold and italic text

### To use Bold in markdown you put 2 asterisk between the words or word you want bold
This is **Bold text**

### To use Italic tect in markdown you put 1 asterik between the words or word
This is *Italic text*

## Userstory-008: Emoticons (has github support)


** Hur man lägger in en emoticon i markdown **  

1. Hitta en emoticon du gillar i detta fall använder jag mig av sunglasses

2. Lägg kolon framför och efter emoticon så det blir såhär

:dinEmoticon:

:sunglasses:

## Userstory-009: Horisontal rulers

Horisontal rulers can be created by using three or more of  *,- or _ 
and by placing them all on their own lines.

You should get something like this


***


---


___

## Userstory-010: Lists

There are a few ways of making lists.

### 1. 

You can also press ctrl+p to do a block selection, and through "veteran speed keyboarding" make lists incredibly fast.

### 2. 

Of course you can still work the same good old ```<ul/><li/>```-way



## Userstory-011: Blockquotes
### Check this one out:

```
Just like DaVinci one said:

> Don't fuck with my commits shorty damn

before he got stabbed to death.
```

Which comes out looking like this;

Just like DaVinci one said:

> Don't fuck with my commits shorty damn

before he got stabbed to death.

## Userstory-012: ER diagrams

You define a Entity Relationship Diagram by rendering them with mermaid, you start by typing three backticks then typing mermaid connected to them, which you also  
end the diagram with but you dont type the mermaid, only three backticks  

Then you make the diagram by defining which type of diagram it is, in this case its an erDiagram.
Here is where you type the different entities and their relationships.
for instance if you write
ENTITY ||--o {SECOND-ENTITY : LABEL  
then you get this

```mermaid
  erDiagram
    ENTITY ||--o{ SECOND-ENTITY  : LABEL
```

Then you can make them more like a diagram by adding more such as this

```mermaid
  erDiagram
    ENTITY ||--o{ SECOND-ENTITY  : THIS-IS-THEIR-LABEL
    CONNECTED-TO-ENTITY ||--|{ ANOTHER-ENTITY : THIS-IS-ALSO-A-LABEL
    ENTITY }|..|{ ALSO-ANOTHER-ENTITY : THIS-IS-ALSO-ANOTHER-LABEL
```

## Userstory-013: Class diagrams
The top compartment contains the name of the class. It is printed in bold and centered, and the first letter is capitalized. It may also contain optional annotation text describing the nature of the class. 
The middle compartment contains the attributes of the class. They are left-aligned and the first letter is lowercase.
The bottom compartment contains the operations the class can execute. They are also left-aligned and the first letter is lowercase.

```mermaid
classDiagram
Animal <|-- Duck
Animal <|-- Fish
Animal <|-- Zebra 
Animal : +int age
Animal : +String gender
Animal: +isMammal()
Animal: +mate()

class Duck{
+String beakColor
+swim()
+quack()
}

class Fish{
-int sizeInFeet
-canEat()
}

class Zebra{
+bool is_wild
+run()
}

```

## Userstory-014: Pie-charts

Since Userstory-014 was not specified, we will here present a pie chart.<br>
"mermaid" and "pie" are the more important key words in this instance.<br>
(You'll also get to choose your fancy title)

```mermaid
pie
    title Hur många idioter?
    "Idioter" : 402
    "Icke-idioter" : 270
    "Övriga" : 87 
```
```
mermaid
pie
    title Hur många idioter?
    "Idioter" : 402
    "Icke-idioter" : 270
    "Övriga" : 87 
```


## Userstory-015: Highlighting certain words

### 1. 

You can either put a mark-tag (w opening/closing tag)

### 2.

You can do it javascript style as well, by highlighting the text by color.

```js
<div style="background-color: #FFFF00">Highlighted text</div>
```

## Userstory-016: Sequence diagrams

To make a sequence diagram you copy these lines and you change them according to what you want it to be

```
mermaid
 sequenceDiagram
    		Alice->>John: Hello John, how are you?
    		John-->>Alice: Great!
    		Alice-)John: See you later!
```
### For example 
## How to make a sequence diagram in markdown

You have to first define that you are going to use mermaid, you do this by typing three apostrophes and then the word mermaid after you type three apostrophes to close when you want to stop using mermaid
You then have to specify which diagram you want to use, in this case we want to use a sequence diagram. 

You have to then define which participants you want to use, in this case we will use John and Alice
To The make them connect to eachother you type: 
Alice -->> John or John -->> Alice

This will result in this:

```mermaid
sequenceDiagram
    Alice->>John: Hello John 
    John-->>Alice: Hello Alice
```
You then have to specify what you want them to say, you do that by using a colon

This will result in this:
```mermaid
sequenceDiagram
    Alice->>John: Hello John, how are you?
    John-->>Alice: Great!
```

## Userstory-017: Classic line breaks

Just like in HTML, you can add < br > tags to put in line breaks.<br> 
I do it regularly in JS, let's try it!<br><br>

It <br><br>
May<br><br>
Look<br><br>
Like<br><br>
This
