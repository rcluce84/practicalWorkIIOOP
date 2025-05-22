# practicalWorkIIOOP
![image](https://github.com/user-attachments/assets/7c8db87a-1cc0-48d1-a636-03e40528e16e)

First of all the zip file from the project was to big for github to let me uploadit so the solution was to add it to drive, create a link and shere the link here, hope this does not affect that much my grade:
https://drive.google.com/file/d/1CLgWy2biIRUWJe_3-TywKPei5vwFIRUG/view?usp=sharing
This is my repository where I developed my solution for the practical work 2 needed to pass the OOP subject.
Table of Contents
Introduction	
Description of the Solution	
Development Decisions:	
Class Diagram	
Problems and challenges	
Conclusión	

Introduction
In this document I will describe the design and development process of a graphical base converter application developed in .NET Maui. The application allows users to authenticate, create their account, recover passwords and a wide range of different number conversions through a user-friendly interface.

Description of the Solution
The solution I opted for was based on a design decision that consisted of 2 different coding approaches. Maui GUI and Logic 

Maui GUI was used to handle the user interactions, input and presentation.
Logic was used to create the code for  the practical work we have been implementing so far.

The Maui part was built with .Net Maui xaml using buttons and grid layout to create a calculator interface.

The user authentication and data storage was done using a json file for storage. I will talk more about this because there were many problems trying to get this to work correctly.

Each conversion was encapsulated in its own class, they were all child classes that inherited from the abstract class Conversion.
Development Decisions:
Each conversion uses its own input validator to ensure that everything is correct. 
The program is done so that it knows how to detect whether the operation requires a specific bit size like the “two's complement” operation does or it simply doesn't. 
The conversion result is displayed dynamically.
The system is supposed to track the numbers of calculations a user performs. (will talk more about this in the problems section).
The inputs that the user decides to put in the calculator for the conversion are taken from a  calculator style interface to simulate pressing a key.


Class Diagram
![image](https://github.com/user-attachments/assets/d603f24a-c8d0-4489-9b5b-b8f834195dff)





Problems and challenges

Integrating the logic project into the MAUi was initially difficult, it required manually dieting project references and understanding how multi-project solutions are structured, (this is something that is not 100% clear to me).

User Data storage via json file. One of the most persistent issues during the development was understanding how user data was stored using json. Even though It works because it stores all the necessary info for the program to work, the exact location of the generated user.json was never entirely clear.
It made it difficult to manually check if data was being saved or updated as expected, but I was able to confirm through the app behavior that everything worked as it should.

Maui being a new and less documented framework was a major problem due to the learning curve of it. I could only attend 1 class regarding this subject due to other academic reasons, so not being able to ask the professor for questions regarding the app made the development take longer than I would have liked. Having to do this, did in fact have its pros and cons. The cons are obvious but the pros were that I learned more about the subject when I had to look into different solutions for other people, videos, courses, etc.

There was this compilation error that kept haunting me during this programming workout. XFC0002, this is caused by incorrect event handlers names or misslinked XAML elements, it took me a while to figure out why this was happening but once I did I was way more careful with my XAMl element linking.
Conclusión
Even thought this was a tedious project to make and due to the difficulties of the project itself, the learning curve mentioned before, and especially the time of the year that we are in, meaning having to compaginate this project with other subjects, I will say that it was an amazing feeling seeing how after all the time spent on it how good it worked. Sure it isn't perfect, there's plenty of things I could have done better like the json file or a prettier more professional design of the app but at the end of the day it works, and with that I'm more than happy.
Even though this was a tedious project, I have to admit that it feels amazing seeing this application come to fruition. The difficulties of the project itself combined with a learning curve produced by the lack of experience with the coding software and the time of year we are in, (studying for exams in other subjects) placed more stress on me than I would have liked but the end result is satisfying. Sure it isn't perfect, there's plenty of things I could have done better like the json file or a prettier more professional design of the app but at the end of the day it works, and with that I'm more than happy.
