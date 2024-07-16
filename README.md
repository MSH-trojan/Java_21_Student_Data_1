# Java_21_Student_Data_1

Introduction:

In this assignment you will create a JFrame application for a university, organizing student data inside a Registrar object. The class corresponding to this JFrame application is called TestStudents. 
The class Registrar contains a single array st[] containing up to 100 objects of Undergrad and Grad type. 

Your Task

Start by writing the class TestStudents as a JFrame application of the size (500,600).  

Inside the constructor TestStudents() create an object rg of Registrar type and use its methods addUndergrad() and addGrad() to create objects of Undergrad and Grad type, which should become the elements of the array st[].  Use the following code:

        Registrar rg = new Registrar ();
        rg.addUndergrad("Jones", 1,"ITEC1000", "ITEC1010", "ITEC1620"); 
        rg.addGrad("Johnson ", "ITEC5260", "Cybersecurity");
        rg.addUndergrad("Jordan", 1.1, "ITEC2610", "ITEC2600", "ITEC2620");
        rg.addUndergrad("Hamza", 1.2, "ITEC3220", "ITEC3230", "ITEC3210");
        rg.addGrad("Adams", "ITEC5710", "Cloud application");
        String s = rg.printReport() + "\n";
        s += "****************************************************************\n";
        s += rg.printAllGrads();
        JTextArea t1 = new JTextArea( s, 80, 40 );
        container.add( new JScrollPane( t1 ) );  

In the same file, below class TestStudents add classes Registrar, Registrar, Student, Undergrad and Grad.  Details are given below. 
First create class Registrar, which has the array st[] and the following methods:
 void addUndergrad(String, double, String, String, String)
 void addGrad (String, String, String) 
 String printReport()
 String printAllGrads()

Classes Undergrad and Grad are derived from class Student.  
Class Student has encapsulated String name.  
Class Undergrad has the encapsulated Strings course1, course2 and course3 and the double fee.  
The class Grad has the encapsulated Strings course and project and the double fee.  
Each class should have a constructor and a method toString() which will return a string that displays all the information shown in the required output window. At the end of each string appears also the fee calculated with the method getFee().

For undergrads at the level 1000 the fee for each course $850, for the level 2000 the fee per course is  $850 times 1.1, while for the level 3000 the fee per course is $850 times 1.2.  
For grad students the fee for the course is $1050 and the fee for the project is $1250. 

Below is the correct output window which shows how to write the toString() methods.

 
