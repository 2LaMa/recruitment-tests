# Questions
**Instructions:** Answer the questions, be concise.

## What is an Object?


Accoridng to the Larousse, an object is every concrete thing, that can be perceived with sight or touch. In Object Oriented Programmation, the "object" refers to an untouchable but still very understandable thing. It can be the agregation of data structures, variables or functions / methods. Often, the object refers to an instantiation of a class, which is the conceptual side of an object : this is like talking about chairs (class), and having in front of you one particular chair (object). As a chair, an object has different attributes and functions : let's say here : 
 + allow one person to sit ()
 + numbers of legs : 4
 + material : wood
 + has_back : yes

Thinking of programmation with objects allows to have a modular and human-understandable code, mostly because of the concept of inherithance. Though, several classes can be represented as children of one class : A chair and a banch can be represented as children of an abstract class that we could call "sitting objects" in which we could set attributes such as 

+ allow one person to sit ()
+ numbers of legs : 4

However, thinking of programming as objects involves a big amount of conceptualization in order not to make mistakes. This way, if your model involves 6-legs-sitting-objects, the previous model may not work and one would like to change it in order to have a nice consistent model.

## Can you explain the difference between include and extend in Ruby?

In order to answer this question I had to check the internet because I am not very knowledgeable in Ruby so far.
So, both are to import module code. The difference is that Include imports this code as a subclass of the original class while Extend imports the code as n instance of the module. This way, if one needs to access attributes of an extended module, it has to be done through the class definition. For an included module it has to be through the original class. This example given by geeksforgeeks is quite clear : 

```
module Geek
  def geeks
    puts 'GeeksforGeeks!'
  end
end
   
class Lord
  
  # only can access geek methods
  # with the instance of the class.
  include Geek
end
   
class Star
    
  # only can access geek methods
  # with the class definition.
  extend Geek
end
   
# object access 
Lord.new.geeks
  
# class access
Star.geeks 
  
# NoMethodError: undefined  method
# `geeks' for Lord:Class
Lord.geeks 
```



## A real estate developer has constructed a more than 100-storey building in the heart of Manhattan. Several months after the inauguration, residents complain about slow elevators, what can the real estate developer do to solve this problem?

In order to answer this problem he should first define its scope of questioning. Can he cut the building in two to have two building of 50 floors? Probably not. Can he fire the residents because they are not happy ? Does not sound like a good solution. So he has two variables that will not change : the residents and the height of the building. It belongs to him to understand why and how residents complain. 

He should first make an open survey in order to understand fully the resident's problem. If this is really about speed, and that those elevators make them late, then he should probably check for new kind of elevators. But if this is all about the feeling of slowness, he could find another solution.

Second, maybe a newer elevator would not fix the problem because it' simply not available / the other elevators are not fast enough to make a difference. Also, the developer might want to avoid spending a lot of time and money in the change of those super long elevators. Then, he might think about ways to make the travel feel shorter, such as the inlay of speakers in the wall to play good music, screens to display some content that would entertain the people, or even games. 
Also, if the elevators do not have mirrors, he should add at least one : it's very important not to feel shut in a box and it feels very weird to be forced to stare at a wall for few moments.

## Is testing a waste of money? Why?

If we talk about code testing, I would quickly answer that testing seems to be a pretty inevitable step if the final product has to be secure, consistent and not buggy. Now if we talk about testing for user interaction, the question is a bit more touchy -even if the answer is the same-. 

Testing might be perceived as a waste of money by some. Indeed, it costs time to organize, money to hire testers, and may lead to backtracking on the project. 

Nonetheless, testing is about to be the opposite of a waste of money, especially if it's done progressively. It is a really sure way to create softwares that will fit to the users, in every sense of the word. In *Rocket surgery made made easy*, Steve Krug gives us some precious pieces of advice for user testing : 

- "A morning a month, that's all we ask" If the testing is done often with a small amount of people, it will not require a lot of time or money, and since the testing will be done often it is not needed to hire people with special skills or knowledge about the project to get out of it with profitable results. 
- "Start earlier than you think makes sense" As said previously, the more iterations, the less design errors. So as soon as there is some content, even if this is a simple prototype that is far away from the final product in mind, it should be tested.
- "When fixing problems, always do the least you can do" It is probable that a session of testing leads toward a scary void of endless possibilities of change, and it is easy to go ahead in a possible direction that will involve a lot of work and time, and might impact previous bases of the project. This way, it is better to find the least-changing solution -the one that asks the least work, while covering properly the problems that have been found-. The problems fixed this way have always to be the most important ones, and the less important have to be fixed and re-tested later.

This is just some ways I think of testing right now but to me these words are enough to convice you that testing is everything but a waste of money.

## Set up a challenge for another candidate in order to test his/her abilities, explain your choice.

A King cake is a pluff pastry filled of frangipane associated with Christian Epiphany. In France it is usual to put a fève inside the cake, and the one who finds it in his/her slice will be the King/Queen. A recurrent issue with this tradition is that that at the moment of cutting the cake the knife hits the fève which breaks the mistery of where it is. What solution(s) would you bring in order to fix this problem ? For each describe the pros and the cons, and think of why it should not have been done before.



This problem involves the creativity and can say a lot about the problem-tackling methods of the candidate. It is quite open and many solutions are possibles. Changes can be made on the side of the baker, of the cake, or  of the eaters (or even elsewhere, who knows). This problem was given to me after my first year of engineer and I remember how proud I was of my first answer, and how amazed I was hearing all the different answers given by my friends.

