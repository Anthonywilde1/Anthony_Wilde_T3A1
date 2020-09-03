# Anthony Wilde, T3A1, Flextrack, Victoria.

## Q1 |Provide an overview and description of a standard source control process for a large project.

#### [Sources]---
1. [label](link)

---

## Q2 |What are the most important aspects of quality software?
Reliability, Understandability, Modifiability, Usability, Portability, Correctness, Efficiency, Testability, Integrity/Security, Flexibility, Reusability, Interoperability, Maintainability.
There are multiple aspects of quality software, often debated with how many are listed, as some aspects can be seen as nested aspects of other aspects. Regardless I see all the aspects that I list below as being important as the removal of them would reduce overall software quality or customer experience with the software.
The imporant aspects are; <u><strong>Usability</u></strong>, <u><strong>Modifiability</u></strong>, <u><strong>Understandability</u></strong>, <u><strong>Reliability</u></strong>, <u><strong>Portability</u></strong>, <u><strong>Correctness</u></strong>, <u><strong>Efficiency</u></strong>, <u><strong>Testability</u></strong>, <u><strong>Integrity/Security</u></strong>, <u><strong>Flexibility</u></strong>, <u><strong>Resuability</u></strong>, <u><strong>Inteteroperability</u></strong> and <u><strong>Maintainability</u></strong>
<strong>Usability:</strong> The aspect that is based around how easy is your software to use, the installation and how well the software runs for a User/consumer. Mainly around the user experience things like; navigation of software and ease of new customers to pick up and start using. An extremely important aspect because Usability drives market forces, if no-one can figure out how to install your software of if your software isnt intrinsic/ easy to learn, people are often not going to give you the time of day to understand your software enough to use it. Essentially aiming for the perfect customer experience.
<strong>Modifiability:</strong>An aspect of quality software that applies to a developer, modifiability is being able to change/modify existing software with new code/systems/plug-ins and not have the software collapse because of it. This is an aspect that is the polar opposite of the fragile code analogy, where your code works but "dont touch it because it might break". If your code collapses because you attempted to add a plugin like AWS or a new system to the software, then your code would not be seen as modfiable.
<strong>Understandability:</strong> This aspect is often refered to by a different name within Coder Academy but the principles of this aspect are the same. DRY(Dont Repeat Yourself) and Indentations are a standard amongst coding languages. We as developers are expected to create code that if another dev was to take over our work or come to assist us that they would be able to understand what was going on because your code was written in such a way that it would be easy to understand what belongs to what or what is assigned to what.
<strong>Reliability:</strong> A reliable code is a code that will run as expected over and over and over again with little to no errors. Reliability is important as the software when it is out on the market will be being used by 100s or 1000s of people. With that in mind you want to ensure your software works reliably for every single customer.
<strong>Portability:</strong> Portability is about using the software on different devices. This could be; 1. Creating something on Linux and ensuring it works for Apple or Windows software. 2.Creating a web app that can be viewed on a desktop, a tablet or a smartphone. This aspect is more concerned with the  access of your software to as many people as possible so it can have the biggest impact. It's important to have good portability because often you want to have as big of a user base as possible.
<strong>Efficiency:</strong> Efficiency is about the performance of a given software on the technology. It is based around concepts like the "Big O notation" and how much computer processing power your software will take up. This is imporant because something that is very demanding on your tech so only people with 16gb of ram and 4 GPU's isn't necessarily a good business model, or something that causes your battery on your phone to drain rapidly will not be well received by users. Personally efficiency is  vital for me as I dont enjoy games and applications that cause my pc to crash or lag really badly, I moved over to consoles specfically for this reason. Efficiency is tied into the overall reception of the software/product you are making.    
#### [Sources]---
1. [label](link)
---

## Q3 |Outline a standard high level structure for a MERN stack application and explain the components.

#### [Sources]---
1. [label](link)
---

## Q4 |A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?

#### [Sources]---
1. [label](link)
---

## Q5 |With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges.

#### [Sources]---
1. [label](link)
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

#### [Sources]---
1. [label](link)
---

## Q9 |Explain data types, using examples from the JavaScript programming language.

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
