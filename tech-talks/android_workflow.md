%title: Android Workflow & Automating All The Things!
%author: @daveshah
%date: 2015-06-03


-> Opinions. Everyone has them... <-
=========

I am not an expert.

I am just a guy with some opinions formed from some experiences.

Your experiences may differ, and I am okay with that.


-------------------------------------------------

-> # You write code right? <-

* You have a workflow. 

* Most of the time you are unaware of it.

* You should become aware.

-------------------------------------------------

-> # So, What Is a Workflow? <-

Context matters. 

Sometimes mine looks like this:

Write a Test-> 
		Make It Pass-> 
				Refactor-> 
						<-Repeat

-------------------------------------------------

-> # So, What Is a Workflow? <-

Other times it might look like this:

Spike->
	Learn->
		Refactor/Stabilize->
						<-Repeat


-------------------------------------------------

-> # So, What Is a Workflow? <-

But there is more...

`git pull --rebase`

(Test -> Implement -> Refactor -> Repeat)

`git add -A . && git commit -m "GPS coordinates are uploaded on save"`

`git pull --rebase`

`./gradlew connectedCheck`

`git push origin master`


-------------------------------------------------

-> # So, What Is a Workflow? <-

And more...

* Manual testing

* Deployment


-------------------------------------------------

-> # There are a lot of details in those tiny little steps <-

* Are my tests manual or automated?

* Are my integration, build, and deployment processes manual or automated?


-------------------------------------------------

-> # I am continually seeking ways to make my workflow more efficient <-

From my experiences, I have learned that:

* The mouse can slow me down.

* Heavy weight tools can slow me down.

## Manual processes are error prone and, more often than not, SLOW ME DOWN.

-------------------------------------------------

-> # If I slow down, get bogged down, or stop to shave a yak, I lose focus. <-

``
						.-'`  (  '.
					.-'         ;  \___      _,
				__.'  )      \'.__.'(:;'.__.'/
		__..--""  		(     '.__{':');}__.'
	.'         (    ;      (    .-|` '  |-.
	/    (       )     )        '-p     q-'
	(    ;     ;          ;     ; |.---.|
	) (              (      ;     \ o  o)
	|  )     ;       |    )     ) /'.__/
	)    ;  )    ;   | ;       //
	( )             _,\    ;  //
	; ( ,_,,-~""~`""   \ (   //
	\_.'\\_            '.  /<_
	 \\_)--\             \ \--\
	  )--\""`             )--\"'
	  '""'                '""'

``

## I have shaved a lot of yaks

-------------------------------------------------

-> # Repetition is wasteful <-

D.R.Y applies to more than just code.

``
	if(timeToAutomate(task) < tolerance(timeToPerform(task),timesPerformed)) {
		automate(task);
	}

``

* note that tolerance is a function of the duration and number of times performed.
* timeToAutomate is a function of knowledge of and skill in the tools available to automate.

## make time to increase your knowledge in and of these tools

-------------------------------------------------

-> # Bottlenecks inhibit and can stop the flow <-

* Manual processes == manual bottlenecks
	- Know your bus factors 
		* Tom the tester
		* Bob the builder
		* Debbie the deployer

If there is a step in the flow of getting your application to production that only
one member of the team can or feels comfortable performing, YOU MIGHT BE DOING IT WRONG.

-------------------------------------------------

-> # Start here: <-

* Reflect on your workflow (Mini "retrospectives", Katas, Pairing)
	- This might be a good time to do a quick Android Kata

* Remember, you are not alone. Our industry is full of schlep work. The open source community loves to get rid of it. You should too.

* Think twice about clicking and configuration. ESPECIALLY if that configuration is not in code.
	+ If you cannot checkout, build, test, and deploy from the command line, you might be doing it wrong.

-------------------------------------------------

-> # It might help if we take a look: <-

# Local build & test
# CI
# Deployment

-------------------------------------------------

# THANKS!

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$_$$$$$$$$$$$$$$$$_$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$__$$$$$$$$$$$$$$_$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$_______________$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$___________________$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$____$$$_________$$$____$$$$$$$$$$$$$
$$$$$$$$$$$$$_____$$$_________$$$_____$$$$$$$$$$$$
$$$$$$$$$$$$___________________________$$$$$$$$$$$
$$$$$$$$$$$$___________________________$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
$$$$_____$$$____________________________$$$____$$$
$$$$_____$$$____________________________$$______$$
$$$$_____$$$____________________________$$______$$
$$$$_____$$$____________________________$$______$$
$$$$_____$$$____________________________$$______$$
$$$$_____$$$____________________________$$______$$
$$$$_____$$$____________________________$$______$$
$$$$______$$____________________________$$______$$
$$$$_____$$$____________________________$$______$$
$$$$$___$$$$____________________________$$$___$$$$
$$$$$$$$$$$$____________________________$$$$$$$$$$
$$$$$$$$$$$$____________________________$$$$$$$$$$
$$$$$$$$$$$$___________________________$$$$$$$$$$$
$$$$$$$$$$$$$$$$$______$$$$$$_____$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$______$$$$$$_____$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$______$$$$$$_____$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$______$$$$$$_____$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$______$$$$$$_____$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$


-------------------------------------------------

