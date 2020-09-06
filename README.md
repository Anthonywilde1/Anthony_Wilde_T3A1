# Anthony Wilde, T3A1, Flextrack, Victoria.

## Q1 |Provide an overview and description of a standard source control process for a large project.

#### [Sources]---
1. [label](link)

---

## Q2 |What are the most important aspects of quality software?
There are multiple aspects of quality software, often debated with how many are listed, as some aspects can be seen as nested aspects of other aspects. Regardless I see all the aspects that I list below as being important as the removal of them would reduce overall software quality or customer experience with the software.
The imporant aspects are; <u><strong>Usability</u></strong>, <u><strong>Modifiability</u></strong>, <u><strong>Understandability</u></strong>, <u><strong>Reliability</u></strong>, <u><strong>Portability</u></strong>, <u><strong>Correctness</u></strong>, <u><strong>Efficiency</u></strong>, <u><strong>Testability</u></strong>, <u><strong>Integrity/Security</u></strong> and <u><strong>Maintainability</u></strong>.</br>
<strong>Usability:</strong> The aspect that is based around how easy is your software to use, the installation and how well the software runs for a User/consumer. Mainly around the user experience things like; navigation of software and ease of new customers to pick up and start using. An extremely important aspect because Usability drives market forces, if no-one can figure out how to install your software of if your software isnt intrinsic/ easy to learn, people are often not going to give you the time of day to understand your software enough to use it. Essentially aiming for the perfect customer experience.</br>
<strong>Modifiability/ Maintainability:</strong>An aspect of quality software that applies to a developer, modifiability is being able to change/modify existing software with new code/systems/plug-ins and not have the software collapse because of it. This is an aspect that is the polar opposite of the fragile code analogy, where your code works but "dont touch it because it might break". If your code collapses because you attempted to add a plugin like AWS or a new system to the software, then your code would not be seen as modfiable. Maintainability is often describing the same ideas as modifiability but with a few minor exceptions, the main one being can you change exisiting code without the introduction of new bugs.Maintaiablity also refers to the ability of the code for being backwards compatible. That being the ability of the code to function on earlier systems/technologies/softwares.</br>
<strong>Understandability:</strong> This aspect is often refered to by a different name within Coder Academy but the principles of this aspect are the same. DRY(Dont Repeat Yourself) and Indentations are a standard amongst coding languages. We as developers are expected to create code that if another dev was to take over our work or come to assist us that they would be able to understand what was going on because your code was written in such a way that it would be easy to understand what belongs to what or what is assigned to what. Another key way for Understandability to be improved are meaningful git messages when  you upload files and also by adding meaningful comments into codes. In javascript a // (double slash) starts a comment in code and another // ends it (or a line break) </br>
<strong>Reliability:</strong> A reliable code is a code that will run as expected over and over and over again with little to no errors. Reliability is important as the software when it is out on the market will be being used by 100s or 1000s of people. With that in mind you want to ensure your software works reliably for every single customer.A good way to make code reliable is to write tests, whether they are automated or manual which I shall talk about later.</br>
<strong>Portability:</strong> Portability is about using the software on different devices. This could be; 1. Creating something on Linux and ensuring it works for Apple or Windows software. 2.Creating a web app that can be viewed on a desktop, a tablet or a smartphone. This aspect is more concerned with the  access of your software to as many people as possible so it can have the biggest impact. It's important to have good portability because often you want to have as big of a user base as possible.Portability can be done by stating certain CSS rules for different screen sizes e.g. Mobile vs Computer vs tablet.</br>
<strong>Efficiency:</strong> Efficiency is about the performance of a given software on the technology. It is based around concepts like the "Big O notation" and how much computer processing power your software will take up. This is imporant because something that is very demanding on your tech so only people with 16gb of ram and 4 GPU's isn't necessarily a good business model, or something that causes your battery on your phone to drain rapidly will not be well received by users. Personally efficiency is  vital for me as I dont enjoy games and applications that cause my pc to crash or lag really badly, I moved over to consoles specfically for this reason. Efficiency is tied into the overall reception of the software/product you are making.</br>
<strong>Testability:</strong>Testing is mandatory part of programming for developers, if your software isnt tested it is viewed as you cant be certain whether the software would work reliably, you need to be able to test that your software works, that any inputs from the user will yield the results as expected.Testing can be done manually, by writing a manual test, either in the code or in text about what you expect an input / output to use. Automatic tests are tests that you can write for yourself with the aid of 3rd party software that will automatically try do what you wrote for the test but try it 1000s of times before either returning a pass or a fail response.</br>
<strong>Integrity/Security:</strong>Software needs to have security, if your application handles private information then secuirty is required, as well as integrity of your software, you dont want to allow people to inject SQL code into your app to break it, giving them access to admin privilege, or you dont want malicious users to break into the database and get peoples private information. While 100% security is impossible, ensuring that you have a healthy balance between security and accessibility is optimal for your software, no-one smart would wish to buy something not from a secured website and you would be concerned with having your private information lifted and used.
      
#### [Sources]---
1. [Softwaretestinghelp](https://www.softwaretestinghelp.com/what-are-the-quality-attributes/)
2. [Silasreinagel](https://www.silasreinagel.com/blog/2016/11/15/the-seven-aspects-of-software-quality/)
3. [chapellassociciates](http://www.chappellassoc.com/writing/white_papers/The_Three_Aspects_of_Software_Quality_v1.0-Chappell.pdf) 
4. [Software Quality Wiki](https://en.wikipedia.org/wiki/Software_quality)
---

## Q3 |Outline a standard high level structure for a MERN stack application and explain the components.

#### [Sources]---
1. [label](link)
---

## Q4 |A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project? 
Security, Testing, UI
A team that is attempting to develop a website for a small business would need to have an understanding of HTML and CSS. I would say that Html experience should be enough to be able to write a page, CSS more so as the CSS will be what the small business is looking at (CSS is valueable as it is the first impressions for most people that count), CSS also allows you to modify the screen for different technologies. A language/web framework such as Ruby and Ruby on rails or Javascript and React which allows you to create multi page websites. The team would need a good understanding of databases aswell because depending on the structure or the website or how big this small business you may need to use a different Database systems( for the sake of this question I will say they need to know PostgreSQL). Aswell as being able to modify a database through the modification of tables within the database. The team needs to also have knowledge of deploying web based apps, usually done as a service that they will have to work out with the small business, this deployment service is important because it is what will keep the website running post production. Without deployment you wouldn't have a working website so to have that knowledge is vital for a web dev. I would also suggest that the team have a good ability to communicate both externally and internally. You want to be able to understand what the business wants and communicate what is possible to them, you also need to communicate who does what for the project, it is a bad use of time to have 5 people all making the same database 5 times, communicating is important! Finally depending on what the business wants, maybe the knowledge/ability to download or use different payment services, or possible verification services well, this being a small app I can possible see both of these things being used however the website could also just be a nice set up that advertises something you need to be in store to get, like a restaurant or driving lessons. But being able to track individual users for things like payment and authentication are common enough that I would want my team to be able to install a system into the website that takes care of that feature aswell. I should also mention that a team should have someone who focus on the UX (User experience design) and that a person on the team shoulld be focused and have the skills to run as many tests as possible for the application, testing is important for development.        

#### [Sources]---
1. [label](I talked to Carl on Slack)
---

## Q5 |With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges.
Ruby, Ruby on Rails, Databases, Deployment, Git hub, Branching, Plugins/addons, Keys, MVC
My project that I did for CoderAcademy, the rails marketplace app. To complete that assessment I had to use alot of knowledge and skills.
Firstly I had to plan out my project using a combination of webtools / planning apps, writing out an ERD(Entity Relationship Diagram) for my ideal database and creating wireframes to have a base design for what my website will look like going forward. I also used a Trello board to plot out my process incase I get lost/ distracted.
With the planning finished I can start the app, using knowledge of the Ruby language and the Ruby on rails to create the app and a knowledge of how Github and Git pushing to create a backup of my project going forward. My knowledge of the MVC(Model, View, Controller) and Databases will have already come in handy by this point and continue to do so. When i create the app i also set up the database for the app, I then add the datatypes from my ERD's to the database in my project. Using my knowledge and skills and what I envision the datatypes to be I can set up dependencies and "null: false" statements to ensure that certain data cant be created without other data being created at the same time. Combining my knowledge of how Databases interact with Models, followed by Controllers and finally Views. Finally being able to deploy my work to a deployment site and ensuring that it works on the app/website that I deployed it to.</br>
While this is just a brief overview of the creation of the app it is important to state that my knowledge and skill with Ruby and Ruby on Rails, which the skill of setting objects/classes/datatypes and setting variables in order to set up working views. This also helped when referring to documentation and understanding what I was reading when it came to Ruby On Rails which took some time and practice. But it was process stated above and my the order in which I went about my tasks that was of the most benefit and left me feeling confident in how I would the project would work out. This skill and knowledge allowed me to do things like modify the class of the devise plug in to better suit my needs, adding a stripe payment API and adding Amazon Web Services(AWS) to my app. These skills helped me to overcome the challenges I faced during the project.        
#### [Sources]---
1. [Self Reflection]
---

## Q6 |With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature.

#### [Sources]---
1. [label](link)
---

## Q7 |Explain control flow, using an example from the JavaScript programming language.

#### [Sources]---
1. [label](link)
---

## Q8 |Explain type coercion, using examples from the JavaScript programming language.
Primative Datatypes, Implicit, Explicit, 3 types; string, boolean, number
Type Coercion comes in many types in Javascript, but before I discuss how I need to state what types can be coerced. Primative data types are any data type in Javacript that is not an object this includes; strings, numbers, booleans(true/false), null, undefined and symbols. I will also discuss Objects, a datatype made up of having other datatypes in it and having the [] square brackets or {} curly brackets.</br>
Type Coercion in Javascript happens in 1 of 3 ways when it is done in the language, type coercion will coerce whatever the datatype is into either; a string, a number or a boolean datatype. This is important to know as if you conerce from any data type you will get a string(words), a number or a boolean(true/false). Type coercion is also done explicitly or implicitly. Explicit type coercion is the use Javascript in built objects to do the coercion for you, an example being we take a value called (val) and we write the inbuilt JS objects Number, Boolean or String. Number(val) would convert the data type explicitly into a number, if the value is a boolean true or false it becomes either a 1 or 0, if its a string the coereced value becomes a NaN or Not A Number(which despite the name is infact a number), if the value was a number in a string '16' then the value will become a number data type. Boolean coercion is easier to understand if (val) is a null, undefined, empty, 0 or false then the Boolean object will return false in its explicit coercion or if its not one of the things I have listed it will return true. The last explicit conversion is the String object, this will convert the (val) into whatever it was but with quotation marks around it, '1', 'true', 'false'.</br>
Implicit conversion is when you use the inbuilt operators of certain data types(such as +, - , &&, || ) aswell as the == sign to coerce data. These operators allow us to do implicit conversion between datatypes within the Javascipt code for example; adding a string(RayMysterio) and a number(619) together coerces the number into a string creating "RayMysterio619" , you can take away a string(althought it must be a number within the string) from a number or a number from a string in both cases it implicitly converts the string into a number value. The operators && or || to compare two or more operators with && only giving a response true if both sides of the operator are true, the || or 'or' operator will look if either of the object's is a true value and return true if it is. These operators use similar and in some cases the exact same amount logic as stated in Boolean explicit conversion. Using the operators causes the value to get passed into a form that works with the operator and then conducting the logic on it. Also == compares to data types in a boolean way e.g 'string' == number  would be false because a string isnt inherently a number UNLESS the string is '12' or another number, the == operator will do these implicit conversions if possible before return whether the types are the same type.  </br>
Finally Objects can be type coerced inside of Javascript but normally isn't done as doing type coercion in the data within an object itself. Hash Objects {} are considered a true boolean value, when its converted to a string it becomes an array stating '[object Object]'. When you try to add to it, it becomes '[object Object]+whatever number you enter'.
Arrays as an object can have operators assigned to them aswell, when you attempt to add a number or string or boolean to an array it becomes a string with the array elements and the number/string/boolean attached to the end. The same goes for explicit conversions of hashes and arrays. It will return true for Boolean(arrays), String will return a string of the array and NaN for number and the same responses as stated above for hashes.
``` '10' + 10 = '1010'
    '10' - 10 = 0
    'beans' - 10 = NaN
    true && 1 = 1
    true || false = true   
    true + 1 = 2
    false + 1 = 1
    "string" + false = "stringfalse"
    Boolean("string") = true 
    Boolean(1) = true
    Number('cheese') = NaN
    Number(true) = 1 
    String(1) = '1'
    String(true) = 'true'
    ('string' && 1)? true:false 
``` 

#### [Sources]---
1. [Source1](https://levelup.gitconnected.com/javascript-the-weird-parts-part-i-data-types-type-coercion-pbr-3ecc751ad62)
2. [Source2](https://www.freecodecamp.org/news/js-type-coercion-explained-27ba3d9a2839/#:~:text=Type%20coercion%20is%20the%20process,Symbol%20(added%20in%20ES6).)
3. [Source3](https://en.wikipedia.org/wiki/Type_conversion#C-like_languages)
4. [Source4](https://medium.com/developers-arena/type-coercion-in-javascript-c973b369b272)
5. [Source5](https://medium.com/front-end-weekly/implicit-coercion-in-javascript-5077ad5510d)
6. [Source6](https://codeburst.io/javascript-essentials-types-data-structures-3ac039f9877b)
7. [Source7](https://levelup.gitconnected.com/javascript-the-weird-parts-part-i-data-types-type-coercion-pbr-3ecc751ad62)
---

## Q9 |Explain data types, using examples from the JavaScript programming language.
Primitive, Symbols, Objects, Arrays, Undefined, null, Functions, 
In Javascript, (and other programming languages) 
#### [Sources]---
1. [label](link)
---

## Q10 |Explain how arrays can be manipulated in JavaScript, using examples from the JavaScript programming language.

#### [Sources]---
1. [label](link)
---

## Q11 |Explain how objects can be manipulated in JavaScript, using examples from the JavaScript programming language.

#### [Sources]---
1. [label](link)
---

## Q12 |Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language.

#### [Sources]---
1. [label](link)
---

## Q13 |For the code snippet provided below, write comments for each line of code to explain its functionality. In your comments you must demonstrates your ability to recognise and identify functions, ranges and classes.

```js
class Car {
  constructor(brand) {
    this.carname = brand;
  }
  present() {
    return 'I have a ' + this.carname;
  }
}

class Model extends Car {
  constructor(brand, mod) {
    super(brand);
    this.model = mod;
  }
  show() {
    return this.present() + ', it was made in ' + this.model;
  }
}

let makes = ["Ford", "Holden", "Toyota"]
let models = Array.from(new Array(40), (x,i) => i + 1980)

function randomIntFromInterval(min,max) { // min and max included
    return Math.floor(Math.random()*(max-min+1)+min);
}

for (model of models) {

  make = makes[randomIntFromInterval(0,makes.length-1)]
  model = models[randomIntFromInterval(0,makes.length-1)]

  mycar = new Model(make, model);
  console.log(mycar.show())
}
```


#### [Sources]---
1. [label](link)
