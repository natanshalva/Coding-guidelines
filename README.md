## Coding-guidelines

Our goal is to build stable and reliable systems. 

In the real world, good coding is not about writing fancy code, but rather about creating stable and easy to maintain applications.

## Simple code 

**1 -   The code must be - SIMPLE !**

	Questions that I need to ask myself when I read the code: 

	1 - Am I sure there isn't a simpler approach to get the task done?

	2 - Can I spot a complicated section in my code?
      ( maybe it is a sign that things are not in the simplest way).

    3- Can I explain in simple words what every block of code does ? 
	If it is too complicated to explain, then maybe it can be dan in a simpler way 

--------------------------------------------------------------------

## Names

**2 - Names are the most important thing in the system:**

A - All name must be meaningful 

All mean: variables, files, class, functions - ALL, with no exception


Examples: 

|  type | Bad  | Good  |
|---|---|---|
| File name  | index.blade.php  | agent_index.blade.php  |
|  File name 2 | AveragePositionController  | AgentAveragePositionController  |

**B -  Names can not be ambiguous


Note about names and search:

We use the Editor search all over the project, **ALL THE TIME!**
Good names are the ones that help us to understand quickly what this code does.

If we look at your code and see ambiguous names, we will reject your code.

--------------------------------------------------------------------------------------


## Commented code. 

Every line of code should to be commented.  

( Except if it log , or super trivial )

Examples: 

// find the user from the DB

$user = User::where('id',98798723)->first(); 

------------------------------------------------------------------------

## Logs 

We are working with loges. We use the logs to find where the bug happens later. In PHP and in Js  - we can find where to start checking very fast with the logs. ( copy the log line and search for it in the project )

PHP : every process or big move must be on info level: 

Example: 
Log::info(‘start billing process’) 

Log::debug(‘Get the agents’ )

On JS : 
Console log for **every** important line of code  !


5 - We do not save keyboard strokes!  

No short versions,  no kids stuff !!  We never save keystrokes, even if it is not necessary for the code, or make the code longer ! 

Examples: 

Bad : 

(Agent::get())? True: false ; 


Good: 

$all_agents = Agent::get();

if(!empty($all_agents)){

	Return true; 

}else{

	Return false; 
} 



 

======================================================

## Coding Standards

**PHP 

Var  = $name_of_var    ( all lowercase with underscore ) 

Class -   ClassName - ( first word, capital - no space between words )

File name :  file_name.php     ( all lowercase with underscore ) 



**HTML 

Class:      name-of-class  

ID :      name-of-id    

Order class - id :  <p  class=”some-class”  id=”some-id” > 


Js

Var : camelCase 


================================================================

When you finish design work on html / css  please check: 

HTML 

1 ) No spelling errors in the code


2) All html tags are closed 

3) No extra HTMl tags in code. 

4) All the html tag are the right one for the task. ( if you not sure, please consult me). 

5) If the part that you are working on has textual typography, we need to be sure to use the appropriate hierarchy. H1 -> h2 -> article -> p - span and so on. 

6) All the images have alt attribute. 

7) images have informative names, with underscore only ( no hyphen sign) .

8) if the image is big, then we need to set the right size of image to every width screen. 

9) All images have to be in the size that they are appearing in the page. 

If the image on screen is 100 px * 100 px  , then the size of image must be 100px * 100px. 

10) All images need to be reduced  weight as much as we can without damaging the quealty. If you are not sure, then please ask the designer what to do about it. 



