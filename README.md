# Anthony Wilde, T3A1, Flextrack, Victoria.

## Q1 |Provide an overview and description of a standard source control process for a large project.
A large project following a standard source control process will have multiple devs working on it, say for example there is a large project being worked on by a company (in this example a buying and selling application). This project will have multiple teams of people/ single people working on individual issues. The project will begin with the creation of a base file system that will have the skeleton file structure of the app (that is the file system but without any of the data within them yet as it hasn't been done), this can be created by anyone but for this example we will call that person the 'merge master'. Everyone working on the project will get the go ahead by the person from github or whichever file storage site you use. The teams of people will 'git clone' the file system to their computers.<br>
These individual devs / teams of people will work on a single aspect of the overall project. For the example lets say that one person is working on the views for the buying pages (the web pages for buying things on the app) and the selling pages of the app is being worked on by a different person. Both groups of people will do a 'git checkout' before they start doing any work on this project, this creates whats known as a 'git branch' on the github server, seperating the work that each group is about to do from each other AND from the original source of the project. Finally once all of these steps have been done can people begin doing their work on the project. <br>
The project for these individuals or groups of people will be much like an individual project from this point, you write some code (for our example the individual was creating the web pages for the buying portion of the application). When they have done some of their work/ all of the work they were tasked with doing in this one area they will go through the standard 'git add' of the files they worked on, the 'git commit' with a meaningful message describing what they did that they are adding to the file system and add it to the server with a 'git push'. Once these files have been pushed to the server (still within its branch) the author of said branch can request a merge/pull request which the 'merge master' from earlier(who can be the same person or a seperate person depending on the project). It is the job of the merge master to resolve all conflicted merges within a project. Ideally the person working on the buying side of the app finished his work before the worker on the selling side finished work on their part, because if another person finished worked before the worker on the buying webpages finished then and this other anonymous person had already merged their work into the main/master branch, then this merge request we are on now would remove the previous authors work because the work being uploaded now is not up to date with the additional work already added to main. The merge master will inform the buying person to update their files and then push again before they agree to merge the new code. However its also possible when there is no merge conflicts that the files automatically get merged, but this is not common. Finally the process is done in this way as to have a clear trail back to when an application was ' working ' and when it stopped working and which part of the code stopped it from working. This also helps to observe which branches of the code dont work effectively together.<br>
This is the standard source control process for a group project, depending on the size what was just explained may in itself just be one branch of an even larger project. The scope may change but the fundamentals of what is going on will not. (e.g if the main branch of my example was itself a branch of a bigger project it would go through the same merge requests and the branches of the example went through)  
#### [Sources]---
1. [github e.g](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)
2. [another control source e.g](https://homes.cs.washington.edu/~mernst/advice/version-control.html#Introduction_to_version_control)

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
A team that is attempting to develop a website for a small business would need to have an understanding of HTML and CSS. I would say that HTML experience should be enough to be able to write a page.<br> CSS more so, as the CSS will be what the small business is looking at (CSS is valueable as it is the first impressions for most people that count), CSS also allows you to modify the screen for different technologies.<br> A language/web framework such as Ruby and Ruby on rails or Javascript and React which allows you to create multi page websites.<br> The team would need a good understanding of databases aswell because depending on the structure or the website or how big this small business you may need to use a different Database systems( for the sake of this question I will say they need to know PostgreSQL), aswell as being able to modify a database through the modification of tables within the database.<br> The team needs to also have knowledge of deploying web based apps, usually done as a service that they will have to work out with the small business. This deployment service is important because it is what will keep the website running post production. Without deployment you wouldn't have a working website so to have that knowledge is vital for a web dev.<br> I would also suggest that the team have a good ability to communicate both externally and internally. You want to be able to understand what the business wants and communicate what is possible to them. You also need to communicate who does what for the project. It is a bad use of time to have 5 people all making the same database 5 times, communicating is important!<br> Finally depending on what the business wants, maybe the knowledge/ability to download or use different payment services, or possible verification services well. This being a small app I can possible see both of these things being used however the website could also just be a nice set up that advertises something you need to be in store to get, like a restaurant or driving lessons. <br> Being able to track individual users for things like payment and authentication are common enough that I would want my team to be able to install a system into the website that takes care of that feature aswell. I should also mention that a team should have someone who focus on the UX (User experience design) and that a person on the team shoulld be focused and have the skills to run as many tests as possible for the application, testing is important for development.        

#### [Sources]---
1. [No source I just talked to Carl via slack)
---

## Q5 |With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges.
My project that I did for CoderAcademy, the rails marketplace app. To complete that assessment I had to use alot of knowledge and skills.
Firstly I had to plan out my project using a combination of webtools / planning apps, writing out an ERD(Entity Relationship Diagram) for my ideal database and creating wireframes to have a base design for what my website will look like going forward. I also used a Trello board to plot out my process in case I get lost/ distracted.<br>
With the planning finished I can start the app, using knowledge of the Ruby language and the Ruby on Rails to create the app and a knowledge of how Github and Git pushing to create a backup of my project going forward. My knowledge of the MVC(Model, View, Controller) and Databases will have already come in handy by this point and continue to do so. When I create the app I also set up the database for the app. I then add the datatypes from my ERD's to the database in my project. Using my knowledge and skills and what I envision the datatypes to be I can set up dependencies and "null: false" statements to ensure that certain data cant be created without other data being created at the same time. Combining my knowledge of how Databases interact with Models, followed by Controllers and finally Views. Finally being able to deploy my work to a deployment site and ensuring that it works on the app/website that I deployed it to.</br>
While this is just a brief overview of the creation of the app it is important to state that my knowledge and skill with Ruby and Ruby on Rails, with the skill of setting objects/classes/datatypes and setting variables in order to set up working views. This also helped when referring to documentation and understanding what I was reading when it came to Ruby On Rails which took some time and practice. But it was the process stated above and the order in which I went about my tasks that was of the most benefit and left me feeling confident in how the project would work out. This skill and knowledge allowed me to do things like modify the class of the DEVISE plug in to better suit my needs, adding a stripe payment API and adding Amazon Web Services(AWS) to my app. These skills helped me to overcome the challenges I faced during the project.        
#### [Sources]---
1. [Self Reflection]
---

## Q6 |With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature.
The project I will be refering to is the T2A2 assessment, which is the Marketplace Project. My skills with wireframing and ERD were the most effective, I was able to use both of these assests to achieve full marks in their respective categories by illustrating very clearly what my website would be like. My ability to discuss what the models of the app would be and the relationships they would have with each other (which was shown in the ERD but also through text) and also describing the method of implementation for the database was precise too knowing how/what to implement into my Database was a mix of good understanding of databases but also the good vision of what I wanted for my database. This was followed up with a Trello board which allowed me to effectively track my progress throughout the creation of my app. I was able to use my skills with third party services effectively, even modifying/tweaking one in particular(Devise) to suit my needs. My skills around the MVC(Model View Controlller) were adequate for this assessment being able to make a well structured website quite easily(although without CSS).<br> The following area's were where I received the average marks or below; High Level Components, Problem solved, User Stories, Code Commenting, Complexity; My ability to describe the high level components of my app received average marks, it was mainly because I wasn't 100% certain on what exactly I was meant to be discussing so I spent minimal time answering the question as I didnt want to get bogged down by the question when I could focus on something else. Next the problem solved criteria was slightly above average and adequate but I could have been more passionate about marketing my app and explaining its reason/neccesity. User Stories were next, I received an okay mark for this task too, mainly I wasn't sure what I was meant to be talking about in my stories, my first iteration had stories that were paragraphs in themselves, followed by a new version that were all one liners but maybe not descriptive enough. Code commenting was a part of my assessments where my marks suffered the most, my comments were sub adequate, while I feel my code commenting was good for the controllers, the models and views had a vast lack of coding that would make it difficult for any other dev but myself be able to pick up from where I left off. There simple wasn't enough commenting to explain my code in certain areas because I was taking my knowledge coming from being the creator of the app for granted.<br> Finally my app was seen in certain aspects (mainly the database, models) were deemed acceptable, but missed receiving full marks with my app not being complex enough. Overall my skills and knowledge that I have listed previously in the past two questions served me well in the assessment, having a good understanding of Ruby on Rails, database access, the overall knowledge of the MVC, my ability to do the "paper work" to show off my designs / planning are skills that lead to me feeling confident and doing well with my product. I think with more iterations I could turn some of the things that I was lacking in this project into strengths for new projects.       
#### [Sources]---
1. [Rubric](https://coderacademy.instructure.com/courses/308/assignments/1618/submissions/3400#rubric)
---

## Q7 |Explain control flow, using an example from the JavaScript programming language.
The control flow is the way in which the computer reads the file it is currently on, this is mostly focused on one file in particular but it is possible to run other files within a file with the proper syntax/language. First off a control flow in Javascript will run from the first line of code to the last line of the code, in that order, everytime, unless specific coding practices are used that cause the code to break this 'first to last' sequence of events. This code that breaks the top to bottom method of the javascript page are called conditional structure. Conditional structure or "Block Statements" because we call the bits of codes executed in them are called blocks, involves such things as "if else" statements, "switch" statements, "while" or "for" loops. These block statements have parameters attached to them followed by a pair of curly braces {}, if the parameters/conditions are met then the computer knows the read the code inside the brackets.<br> First we have the if - else block, this block can be chained (done multiple times) by first using some of the information already avaliable on the page, you start an if- else statement with an if key word followed by an expression that is a Boolean value (that is whatever is in the parenthesis must equal to a true or a false e.g if (8 > 4)) and only if this condition is met then it will read the code within the adjacent curly braces, or else it will skip over it, you can follow up this if statement with an else if statement if you wish to check multiple conditions or do separate things if the values you send in meet different requirements, finally you can use an else block at the end which is used if the code doesnt meet any of the previous statements you have written, the language knows to skip over any and all blocks that it doesnt meet the requirements to use, skipping the 'top to bottom' flow by shortcutting and reading only what is required.<br> Switch statements work similiarly to if else statements, they are used if a conditional was to have multiple answers, it is a better practice to use switch statements to if else statements if you want a single expression to have multiple pathways (this will be written in code further down the page). We also have while/for loop blocks that allow you to repeat a specific block while certain conditions are met, or for every element in an expression. This means that the code within the adjacent curly brackets will be run as many times as is needed, (for while loops, it is until the expression in the parenthesis follow the while keyword is no longer true, for "for" loops it runs the loop until the for loop has gone through all data it has been given). These loops/ blocks also have a few escapes to get the computer to stop reading through it and continue on reading the program from top to bottom, after the block with the escape in it, the keyword "break" when used in these blocks immediately causes the computer to stop reading where it was and go back out of the block scope. Theres also a continue keyword but this doesnt affect the control flow its used to continue while / for loops.<br> 
Finally the other part of control flow that breaks the top to bottom reading process that is factory default is the idea of 'hositing'. Hoisting is a tricky concept. "A strict definition of hoisting suggests that variable and function declarations are physically moved to the top of your code, but this is not in fact what happens. Instead, the variable and function declarations are put into memory during the compile phase, but stay exactly where you typed them in your code." That is to say that hoisting is the ability for Javascript to "skip" or locate functions/ methods further down the page from where the computer is reading(in its top to bottom approach) to hoist the information it needs to allow the functions/methods to succeed, this is to allow the script/page to run without crashing if you write a function after you have already made calls for that function to be used earlier within the page (this will be explained in the written examples). Hositing is odd in that it works in very specific technical way and if this isn't met then the machine will define things as undefined or error out because it doesnt have the right information or can't do what you want it to do.

```js
(Please treat all code seperated by ----- as if they were on seperate pages)
let a = 10
console.log(a)
let b = 20
console.log(b - a)
/*------------------------------------------------------------------------------*/
if else blocks 
let x = 15
if (x < 14) {
  console.log("this will be skipped because x is greated then 14)
} else if (x = 15) {
  console.log("after skipping first block this block will run because x is 15)
} else {
  console.log(you could run something here if x doesnt meet either of the first two conditions)
}
/*------------------------------------------------------------------------------*/
/*switch statement*/
let console = "nintendo"
switch (console) {
  case "xbox":
    console.log(I guess you could play Halo but not much else);
    break;
  case "playstation":
    console.log(remember the halo killer Killzone, best to stay forgotten);
    break;
  case "nintendo":
    console.log("NINTENDO 64 OMG");
    break;
}
console.log(this happens after the switch console block)    /*p.s the case for xbox and playstation wont be read as we 
can see that console is nintendo.
/* ----------------------------------------------------------------------------- */
/* while / for statement */
let i = 0
while ( i < 5 ) {
  console.log(i);         #this runs a code that will print the numbers 0-4 to console before stopping 
  i++                      when the i is no longer less than 5
}

let array = ["a","b","c","d"]
for (x in array) {
  console.log(array[x])   prints a b c d, before stopping
}   

/*------------------------------------------------------------------------------*/
/*break keyword*/
let x = true 
if (x == true) {
  console.log(before the break)
  break;
  console.log(after the break)  # this will not run due to break
}

/*------------------------------------------------------------------------------*/
/*hoisting*/ 

console.log(fun()) # this will console.log the function of fun despite function being below it

x = 3

if (x < 2 ) {
  console.log( this code exists to demonstrate that hoisting skips past it to find the function before returning to the top);
}

const fun = () => {
  console.log(I am having fun)
}

```

#### [Sources]---
1. [Hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)
2. [Control Flow](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference#Control_flow)
3. [Control Flow2](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow)
4. [Control Flow + error handling](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)
---

## Q8 |Explain  strict definition of hoisting suggests that variable and function declarations are physically moved to the top of your code, but this is not in fact what happens. Instead, the variable and function declarations are put into memory during the compile phase, but stay exactly where you typed them in your code.type coercion, using examples from the JavaScript programming language.
Type Coercion comes in many types in Javascript, but before I discuss how I need to state what types can be coerced. Primative data types are any data type in Javacript that is not an object this includes; strings, numbers, booleans(true/false), null, undefined and symbols. I will also discuss Objects, a datatype made up of having other datatypes in it and having the [] square brackets or {} curly brackets.</br>
Type Coercion in Javascript happens in 1 of 3 ways when it is done in the language, type coercion will coerce whatever the datatype is into either; a string, a number or a boolean datatype. This is important to know as if you coerce from any data type you will get a string(words), a number or a boolean(true/false). Type coercion is also done explicitly or implicitly. Explicit type coercion is the use Javascript in built objects to do the coercion for you, an example being we take a value called (val) and we write the inbuilt JS objects Number, Boolean or String. Number(val) would convert the data type explicitly into a number, if the value is a boolean true or false it becomes either a 1 or 0, if its a string the coereced value becomes a NaN or Not A Number(which despite the name is infact a number), if the value was a number in a string '16' then the value will become a number data type.<br> Boolean coercion is easier to understand if (val) is a null, undefined, empty, 0 or false then the Boolean object will return false in its explicit coercion or if its not one of the things I have listed it will return true.<br> The last explicit conversion is the String object, this will convert the (val) into whatever it was but with quotation marks around it, '1', 'true', 'false'.</br>
Implicit conversion is when you use the inbuilt operators of certain data types(such as +, - , &&, || ) aswell as the == sign to coerce data. These operators allow us to do implicit conversion between datatypes within the Javascipt code for example; adding a string(RayMysterio) and a number(619) together coerces the number into a string creating "RayMysterio619" , you can take away a string(althought it must be a number within the string) from a number or a number from a string in both cases it implicitly converts the string into a number value.<br> The operators && or || to compare two or more operators with && only giving a response true if both sides of the operator are true, the || or 'or' operator will look if either of the object's is a true value and return true if it is. These operators use similar and in some cases the exact same amount logic as stated in Boolean explicit conversion. Using the operators causes the value to get passed into a form that works with the operator and then conducting the logic on it. Also == compares to data types in a boolean way e.g 'string' == number  would be false because a string isnt inherently a number UNLESS the string is '12' or another number, the == operator will do these implicit conversions if possible before return whether the types are the same type.  </br>
<br>Finally Objects can be type coerced inside of Javascript but normally isn't done as doing type coercion in the data within an object itself. Hash Objects {} are considered a true boolean value, when its converted to a string it becomes an array stating '[object Object]'. When you try to add to it, it becomes '[object Object]+whatever number you enter'.
Arrays as an object can have operators assigned to them aswell, when you attempt to add a number or string or boolean to an array it becomes a string with the array elements and the number/string/boolean attached to the end. The same goes for explicit conversions of hashes and arrays. It will return true for Boolean(arrays), String will return a string of the array and NaN for number and the same responses as stated above for hashes.
```js 
    '10' + 10 = '1010'
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

In Javascript, (and other programming languages) there are several unique data types that we used to break down data into categories that help distinguish what the data is. These Datatypes are Numbers, Strings, Booleans, Objects, Functions, Null, Undefined, BigInt, Symbol and Undefined. The following Datatypes listed; Numbers, strings, booleans, undefined, bigint, symbol are what we refer to as primitive data types. They are called primitive because they at any one time can only hold one type within them. A good example is that whenever a string, number or boolean is used it will only return another string number or boolean. Below is an example of a Boolean primitive data type it demonstrates how only one data type (which in this case is the Boolean true) can be held within the Boolean class. In this class it is the Boolean data type, the same goes for the Number data type or the string data type.<br> Primitive data types are incapable of storing anything bar their own data type inside.  
```js 
    Boolean(true) = true
    Boolean(1) = true
    Boolean('string') = true
    Boolean(1+2) = true
```
 Undefined is a primitive datatype as it can only be undefined as long as a datatype has yet to be defined. As of yet, it carries the same logic as before, something can't be undefined and a number, undefined would most often be seen if you forgot to assign a variable an actual datatype and when you do undefined ceases to exist.<br> BigInt is another primitive data type, like all primitive data types it can only store one value at a time, BigInt is used as the ES6 Docs describes 'The BigInt type is a numeric primitive in JavaScript that can represent integers with arbitrary precision. With BigInts, you can safely store and operate on large integers even beyond the safe integer limit for Numbers.' This means that BigInt is most commonly used when a number is too large for the Numbers datatype which roughly means its outside of a physical human beings scope.<br> The last primitive data type is the Symbol datatype, Symbols are again only capable of holding one value, what symbol does is create unique instances of a value which even if they are the exact same as another value will equal false due to it being unique.
```js
 let sym1 = Symbol(123)
    let sym2 = Symbol(123)
    (sym1 == sym2) = false
    let bignum = 123456789n ** 204n
    let x;
    console.log(x); = undefined
```
Finally we can start talking about non primitive datatypes, that is data types that can store more then one value within them at any one time and dont neccessarily overwrite old data to do so. The ES6 documentaion calls the datatypes "structural", other people have called them containers or dictionaries even. This is because the datatype acts like a large container/structure that holds within it smaller data types, which can also be nested within those objects, I'll explain what I mean better as I go through each type of data.<br> Arrays are a structural data type that are most commonly defined by their square brackets [], Arrays are capable of holding any of the primitive data types within them, as well as being capable of storing other arrays within them.<br> The other structural object in Javascript is the hash object, like the array it is capable of storing all between its {} curly braces, even smaller hash objects or arrays! Often the hash objects use symbols to identify the data types within it making it easier to call the data from inside the hash object.<br> Both structual datatypes can be iterated through, that is to be searched through for specific data that can be returned to the user who wanted them.<br> Another data type that is considered in this structual data mindset is the Function, while it itself is not an object its still structural in that it does store other things inside it, often code snippers and data types that are used together to provide answers that the inputter/coder is looking for.<br> Structured objects have numerous inbuilt methods/functions that a programmer can use to do multiple different things to the objects involving modifying the data, adding new data, removing data, searching through the data etc. 
```js 
    let arr1 = [1, 2 , 3 , 4 , 5];
    let arr2 = [[1,2],[3,4]];
    let hashobjectexample = {
      symbol: "string1"
      key: "another name for symbol"
      key2: 1234
      key3: {
        key4: true
      }
    };
    let x = 1
    function example = (num) => {
      return x + 1
    };
```
The last data type is Null, datatype null is considered a primitive datatype, as it can only be one thing, null. However datatype null only exists naturally when you are in the process of trying to call or reference another data type(from a structured data type) and it failed because the data type does not exist, for example in  my has object above if I tried to call information from a key5, key 5 does not exist and therefore would return null. If I tried to obtain an item from the above arrary arr1 and the index of 7 ( the 7th item in the array) that item does not exist and so they will return null. Outside of these referencing errors the only time null appears is when you as the programmer would assign null to an object/data type yourself


#### [Sources]---
1. [Datatype1](https://www.tutorialrepublic.com/javascript-tutorial/javascript-data-types.php#:~:text=There%20are%20six%20basic%20data,objects%20are%20composite%20data%20types.)
2. [Datatype2](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
3. [Datatype3](https://developer.mozilla.org/en-US/docs/Glossary/Undefined)
4. [Datatype4](https://developer.mozilla.org/en-US/docs/Glossary/Symbol)
5. [Datatype5](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
6. [Sauce6](https://developer.mozilla.org/en-US/docs/Glossary/Function)
7. [Sauce7](https://developer.mozilla.org/en-US/docs/Glossary/Null)


---

## Q10 |Explain how arrays can be manipulated in JavaScript, using examples from the JavaScript programming language.
The array object in Javascript has many inbuilt methods that allow us (the programmer/developer) to manipulate the array. First off, a key defining factor between methods is whether the method that is manipulating the array is 'mutating' or 'non mutating', the main difference between the the two is that a 'mutating' method will change/mutate the array, as in the changes made through the method become permanent to the array for the rest of the script/page/flow, where as a non mutating method will return the same value as some of its mutating counter parts but not remove them from the original array.
```js
/*Mutating Array*/
let arr1 = [1,2,3,4,5]
arr1.push(6) = [1,2,3,4,5,6]
console.log(arr1) = [1,2,3,4,5,6]

/*Non Mutating Array */ 
let arr1 = [1,2,3,4,5]
arr1.concat(6) = [1,2,3,4,5,6]
console.log(arr1) = [1,2,3,4,5]
```
Above we see similar code, however the mutating method keeps the new array created by the adding of another number (mutating it) and when we log the arr we can see that, in the non mutating example the 6 is loss in the console.log because it was a non mutating method. Meaning it doesnt change the array permanetly.<br>
There are many methods within Javascript to manipulate arrays. Adding methods; push, unshift( which are mutating) and concat(not mutating), these methods add additional values to the front or back of the array, you "push" the value to the end of an array(concat does this without mutating), you can 'unshift' a value to the start of the array. The remove methods are; pop, shift, splice, slice, filter, which pop,shift and splice are mutating. Pop removes the value from the end of the array (it returns this variable to you, but its gone from the array), Shift does the same as pop but at the start of the array. Splice allows you to remove any number of items from a starting point based at an index in the array you specify and an end point( this means that splice can remove 1 or many items from the array, aswell as the entire array) and returns these items, also splice can also add elements to any part of the array aswell. Splice is mutating also! Slice is a non mutating counter part for splice (meaning it does the same thing bar removing the item from the array permanetly). Filter is the other non mutating removal method, it iterates through your array (it goes through it one by one) and depending on what you decided to filter by, it will remove all elements of an array that do not meet your filter and returns the array. <br>Finally another way to manipulate arrays comes from the iterator methods, while these methods dont mutate the array, you can return instructions to create new arrays that have different values based off your original array. Map and forEach are both methods that iterate. Map returns the new value of what you decided to do in map while forEach does not, neither of these are mutating, you would have to save the changes to a new variable.<br> The final manipulating method I will talk about is reduce, it allows you to execute a function on all the items of an array and then it returns the end product. It is a non mutating method.

```js
let arr1 = [1,2,3,4,5]
arr1.push(6)/* = [1,2,3,4,5,6]*/
arr1.unshift(0) /*= [0,1,2,3,4,5,6]*/
arr1.concat(7) /*= [0,1,2,3,4,5,6,7]*/
console.log(arr1)/* = [0,1,2,3,4,5,6]*/
arr1.pop() /*= [0,1,2,3,4,5] /*(returns 6) */
arr1.shift() /*= [1,2,3,4,5] /*(returns 0)*/
arr1.splice(1, 0, 1) /*= [1,1,2,3,4,5] 
arr1.splice(1,1) /*= [1,2,3,4,5] (returns (1)*/
arr1.slice(1,1) = /*[1,3,4,5] (returns 2)*/
console.log(arr1) /*= [1,2,3,4,5] (slice doesnt mutate)*/
arr1.filter(x => x > 2) /*= [3,4,5] (doesnt mutate)*/
arr1.forEach(x => x +2 ) /*= 3 , 4 , 5 , 6 , 7 (doesnt mutate also returns each value seperately)*/
arr1.map(x => x + 2 ) /*= (3, 4, 5, 6 , 7) (doesnt mutate original array)*/
arr1.reduce((acc, val) => { return acc+ val})/* = 16*/
console.log(arr1) = [1,2,3,4,5] /*(reduce doesnt mutate)*/
```

#### [Sources]---
1. [Mutate vs not mutates](https://lorenstewart.me/2017/01/22/javascript-array-methods-mutating-vs-non-mutating/)
2. [Array MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#Static_methods)
---

## Q11 |Explain how objects can be manipulated in JavaScript, using examples from the JavaScript programming language.
Objects the basis of object oriented programming, has numerous ways to manipulate data, several built in methods to the object class can be applied, as well as manipulation of the data inside of the object requiring you to be able to navigate your way through to the object which is another form of manipulating the object.<br>
Object has a few default methods that come for all objects that can be applied. They have a wide ranging of effects, I will talk about Object.keys(), Object.values(), Object.entries(), Object.seal(), Object.freeze(). Keys as a method will give you an objects keys, in objects, key values are a paired part of data most oftenly a Symbol(key) and its associated value(which can be any other data type), what .keys does it return the keys part of the object, however it does not go past the initial level of an object, meaning that any nested keys(keys within keys) will not be put into the array, its important to add that this method doesnt mutate anything just shows you the keys. .values() does the same as the keys method just with the values and not the keys, it also prints them to an array, it also is important to add this method will return the entire object(an array/ hash) that is associated to a key, with the key still within it. .entries() is similiar to keys and values, it does both at once and creates an array of arrays that has the key value pairs paired up in their own individual arrays.<br> All three methods that I just listed are helpful if you are unsure what the object you are working on has and cant access where the object is stored.
.seal() and .freeze() are two other class Object methods that help to STOP the manipulation of data. .seal "preventing new properties from being added to it and marking all existing properties as non-configurable. Values of present properties can still be changed as long as they are writable." This means that you will be able to change the value of any key in the object, but you cant remove keys or functions, add key + value pairs to an object and finally wont be able to delete the object. .freeze() does the exact same as .seal but it also stops the modifying of values too, making it an object with "read only" privlideges.<br> 
Other manipulations of objects include the delete operator for objects. Calling values with getters and setting values with setters. Starting with getters, the getters refer to calling data from within the object by using functions within the object. Combining the 'this.' which allows you to access any of the keys within the object and then using a getter method, allows you to pull the data through the object and to the console. Setters or set functions, are inbuilt object functions that you can declare that allow for the manipulation of data through the console. This is one of the main ways that a person can manipulate an object, setters also emulate one of the important ways that we can change values in objects, that is by 'objectname[existingkey] = newvalue', we can also add new key value pairs with the same format 'objectname[newkey] = newvalue' , also using an operator when you call a key (object[key]) allows you to do some of the type coercions preveiously stated in earlier questions. Finally the delete operator when called on a objects key through the correct syntax (objectname[keyname]), will remove that objects key and value from the object. 
```js
let obj1 = {
  a: 1,
  b: 2,
  3: 4,
  name: 'anthony'
  nested: {
    nestedkey: "Wow"
  }
}
Object.keys(obj1) /*= [ a, b, 3, name, nested]*/
Object.values(obj1) /*= [ 1, 2, 4, 'anthony', {nestedkey: "Wow"}]*/
Object.entires(obj1) /*= [[a , 1], [b, 2], [3, 4],[name, 'anthony'], [nested , {nestedkey: "wow"}]]*/
Object.seal(obj1)
delete obj1.a /*= Unable to delete due to seal */
obj1.a = 2 /*(okay because this is seal not freeze) */
Object.freeze(obj1)
obj1.a /*= 4 ---- unable because object is frozen*/

let obj2 = {
  a: 1,
  b: 2,
  c: 3
  get getexample() {
    return this.a + this.b + this.c 
  }
  set setexample(x) {
    this.a = x
  }
}

obj2[d] /*= 4 (obj2 now has an additional key value pair)*/
obj2.getexample /*= 6*/
obj2.setexample(5) /*---- 'a' key now has a value of 5 through setter function*/

```
#### [Sources]---
1. [MDN DOCS](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
2. [DELETE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/delete)
3. [Freeze!](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/freeze)
4. [NON-MDN](https://medium.com/infancyit/javascript-object-manipulation-5d1145cf06ef#:~:text=JavaScript%20is%20designed%20on%20a%20simple%20object%2Dbased%20paradigm.,and%20value%20can%20be%20anything.) 
---

## Q12 |Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language.
JSON or Javascript Object Notation is a separate file type to standard JS. It is a text based file that has an object written in text (that is quotation marks "") and besides that important point the text inside of a JSON is written to be exactly the same as a standard Javascript Object ({} curly braces) It is also possible for a JSON to be an array or multiple arrays. A JSON has nested objects/arrays within it. Manipulating JSON's is fairly simple in it follows the same ideas as writing and manipulating of a regular object with a few slight differences. I will discuss the following; Creating JSON(stringify), Deleting JSON, Calling Json(parsing), Iterating through a JSON, Object Class methods, Array Class methods and dot notation.</br>
Creating JSON is simple enough, we can create a .JSON file and write in as many objects or arrays or both as you want, as long as all the keys are "strings" and you start the file off with a '{ or ['. Next if wanted to create an object within a JS script (that was mentioned in the previous question) we can take the object that we saved to a variable and pass it the method stringify(). Stringify takes an object as its parameter and returns the 'string'-ify version of the object (that is the same object with all key/values as strings). This new object can then be written into a separate JSON file using node and a few key words (fs which is file system and .writefile, followed by the object) and you've created an object that is now a JSON file!. Additionally you can add object key/values through the standard object ways (object.key = value or object[key] = value).</br>
Deleting JSON is also similiar to a standard JS object, first off the one that stands out, if you want to you can just delete the text from the JSON file. JSON objects can be deleted or removed in the same ways as suggested above, that is through the delete command or by doing things like splicing(pop, shift etc) or inserting new values into the keys.</br> 
Calling JSON is the main area where JSON is used, you can call JSON files into your webpages through script and then use them on that page to show alot of data while keeping the webpages clean and the data in a separate file. The main way we call a JSON object or Parsing the JSON. The JSON has a method called parse() that returns a JSON object as a standard Javascript object. With parse you can call an object that has been stringified on the same page, aswell as a separate file within the same file system. Once the object has been called we can assign it a variable and manipulate it further. Whether its JSON or Object. </br>
Once an object has been called/parsed from within the same file/separate file we can iterate through it using the same methods that we mentioned above while and for loops can be used on a JSON object, its important to note that a JSON object does not have to be un-strung to be iterated through or added/delete from, the for and while loops are important as its the only way we can loop through  an object, but through using the loops we can call the data within. This can be challenging when there are a mixture of arrays and objects it is still possible to sift through the data to get to where you want to be. JSON arrays can be iterated through with a forEach and Map method.</br>  
Another way to call a JSON is by using the Object.keys or Object.values methods, or with the calling of the element within the object e.g foo.bar["string"] This is because a JSON behaves like a regular object just with strings in place of all keys and values. The .keys or .values method will behave the exact same as stated in the object question, it will return the keys of the object or the values of the object, but it will be in strings. In this way JSON behaves the exact same when it comes to calling objects as a regular object.<br> The other object-like data type in a JSON is an array, these arrays, while containing entirely strings or string key value pairs, can be iterated through and push spliced shifted added to as any other array in javascript. JSON converts the data into strings but doesnt inhibit the object from being worked upon as it was previously except for the data types themselves(as in all data within is now a string until converted back).</br>
Finally because of the nature of objects in javascript and in JSON, we can access data directly if we know how it was formed, that is to say if we want to reach a key value pair 3 nests deep we can, as long as we state the objects name and then chain the keys until we reach the one we need. e.g object.chain1.chain2.key = value OR object.chain1.chain2[key] = value. JSON allows for the same manipulation of data that we would use for a standard Javascript object with a few additional file transferance capabilities that allow for a wider range of use of objects for things like APIs.

```js
let obj1 = {a: 1, b: 2, c: 3}
JSON.stringify(obj1) /*(now obj1 = "{"a": 1, "b": 2, "c": 3}")*/
obj1["a"] /*= 1*/
obj1.b /*= 2*/


for (x in obj1) {console.log(x)}/*  (console would log a, b ,c)*/
 for (x in obj1) {console.log(obj1[x])} /*(would log 1,2,3)*/
let obj2 /*= {one: 9, two : [1,2,3,4,5], three: 8 }*/

JSON.stringify(obj2) /*= '{"one":9,"two":[1,2,3,4,5],"three":8}'*/
obj2.two.map(x => ( x + 1)) /*= [ 2, 3, 4, 5, 6 ] iterating through an array in JSON*/
delete obj2.two
obj2 /*= '{"one":9, "three":8}'*/

let obj3 = {onelevel: {twolevels: {threelevels: "you found me!"}}}
JSON.stringify(obj3) /* = '{"onelevel":{"twolevels":{"threelevels":"you found me!"}}}' */
obj3.onelevel.twolevels["threelevels"]/* = 'you found me!"*/



```

#### [Sources]---
1. [MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON)
2. [other MDN](https://mossgreen.github.io/JSON-manipulation-with-javascript/)
3. [Other other MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON/parse)
4. [Source4](https://www.w3schools.com/js/js_json_stringify.asp)
---

## Q13 |For the code snippet provided below, write comments for each line of code to explain its functionality. In your comments you must demonstrates your ability to recognise and identify functions, ranges and classes.

```js
class Car { /*establishes that this is a Class Object allowing you to create objects/data that have code to go along with it */
  constructor(brand) { /*this is the initializer of the object, the thing that happens on creation, it can require parameters i,e brand*/
    this.carname = brand; /*The parameter brand from the constructor  it is assigning the variable carname with the value of brand. 'this.' is added to the start of carname to allow carname to have object scope, that is the ability to be used outside the constructor curly brackets and anywhere within the Car brackets */
  }
  present() {  /* a method created in for the class Car */
    return 'I have a ' + this.carname; /* return the string I have a and whatever the value of carname is from the constructor, because this was called in the constructor and here the method works */
  }
} /* end of car object block */

class Model extends Car { /* a new class Model that inherits from the class Car  */
  constructor(brand, mod) { /* the initializer of the object, it has 2 parameters, brand and mod  */
    super(brand); /* super calls the parents constructor method, allowing us to use the same brand from the Car class here, we also get access to all methods from the Car class through this super + the extends keyword earlier */
    this.model = mod; /*a second parameter for creation of this Model Object, it has object scope due to the this.model that the parameter mod is assigned to */
  }
  show() { /* a method belonging to the Model class only */
    return this.present() + ', it was made in ' + this.model; /*when the method is used it returns a string starting with a method inherited from the Car class present and followed by a string and finally calls the model from the Model objects creation it puts it all together with string concattenation */
  }
} /* end of model object  */

let makes = ["Ford", "Holden", "Toyota"] /*an array called makes that was created using lets, allowing for modifiability it has 3 items within the array 3 strings named after car brands */
let models = Array.from(new Array(40), (x,i) => i + 1980) /*assigns an variable called models from an Array, Array.from will return whats in the paraenthesis after it to an array. the new Array code creates a new array the (40) in parenthesis will create 40 undefined elements, (x,i) it iterates through the array of 40 undefined elements, x is the iterator and i is the value of the element, it takes on the value of the array.length i.e array[0] = 0, so it goes 1980, 1981, 1982 */

function randomIntFromInterval(min,max) { // min and max included, a function called randomInt.... it has 2 parameters min and max */
    return Math.floor(Math.random()*(max-min+1)+min);/*returns a number that is rounded down, the number is a random number that is the value of max-min + 1 + min) math .random returns a random number between the value from the sum to the right of it */
}

for (model of models) { /* a for loop for iterating through the array of data in models, (40 times as there are 40 data entries created in the array earlier) */

  make = makes[randomIntFromInterval(0,makes.length-1)] /*create a variable make that gets an element from the makes array through the use of the function and feeds the  function a min of 0 and a max of the makes array length -1 */
  model = models[randomIntFromInterval(0,makes.length-1)] /* creates a cariable that gets an element from the models array it does this through the same function and feeds it the exact same min and max values, 0 and makes.length -1 please note this is makes array and NOT the models array that is the max value, causing the answers to be between the values 1980 - 1982 */

  mycar = new Model(make, model); /* assigns a variable mycar that creates  a new Model object using the variables make and model gotten above you can see in Model that the constructor wants different named parameters however these are just placeholder names they dont explicitly needs to be brand and mod*/
  console.log(mycar.show()) /*console logs the results of the mycar variable with the method show from the model class talked about above, this prints to the console, I have a make, it was made in model, finally this will happen 40 times before finishing  as the array models is 40 elements long */
}
```


#### [Sources]---
1. [https://www.w3schools.com/JSREF/jsref_class_super.asp](https://www.w3schools.com/JSREF/jsref_class_super.asp)
2. [https://www.w3schools.com/js/js_this.asp](https://www.w3schools.com/js/js_this.asp)
3. [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from)
4. [https://stackoverflow.com/questions/3895478/does-javascript-have-a-method-like-range-to-generate-a-range-within-the-supp](https://stackoverflow.com/questions/3895478/does-javascript-have-a-method-like-range-to-generate-a-range-within-the-supp)
