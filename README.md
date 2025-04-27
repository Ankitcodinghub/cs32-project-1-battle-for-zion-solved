# cs32-project-1-battle-for-zion-solved
**TO GET THIS SOLUTION VISIT:** [CS32 Project 1-Battle for Zion  Solved](https://www.ankitcodinghub.com/product/cs32-project-1-battle-for-zion-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;86782&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;4&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (4 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS32 Project 1-Battle for Zion&nbsp; Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (4 votes)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
Project 1: Battle for Zion

The appendix to this document is the specification of the last CS 31 project from a previous quarter. We will provide you with a correct1 solution to that project. Your assignment is to (1) organize the code for the solution in appropriate header and implementation files, and (2) implement a new feature.

You should read the appendix now. It describes a game in which a player has to escape from robots in an arena. You will be working with this code that implements the game. Notice that it is a single file. (Just so you know, the way we tested its correctness is similar to how we’ll test the correctness of the programs you write in CS 32.)

Organize the Code

Take the single source file, and divide it into appropriate header files and implementation files, one pair of files for each class. Place the main routine in its own file named main.cpp. Make sure each file #includes the headers it needs. Each header file must have include guards.

Now what about the global constants? Place them in their own header file named globals.h. And what about utility functions like decodeDirection or clearScreen? Place them in their own implementation file named utilities.cpp, and place their prototype declarations in globals.h.

The Visual C++ 2019 and the Xcode writeups demonstrate how to create a multi-file project. From the collection of the eleven files produced as a result of this part of the project, make sure you can build an executable file that behaves exactly the same way as the original single-file program.

Add a Feature

If you try running the updated programs (the Windows version, the Mac version or the Linux version of the full game, and the Windows version, the Mac version or the Linux version of the smaller version of the game), you’ll see they have one new command you can type: p for Previous. This command shows you how many turns the player has been on each grid point (not counting the player’s initial placement on the grid): dot means 0, a letter character A through Y means 1 through 25 times (A means 1, B means 2, etc.) and Z means 26 or more times.

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column"></div>
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
Your task is to implement this functionality. You will need to do the following: Define a class named Previous with the following public interface:

<pre>     class Previous
     {
</pre>
<pre>       public:
         Previous(int nRows, int nCols);
         bool dropACrumb(int r, int c);
         void showPreviousMoves() const;
</pre>
};

The constructor initializes a Previous object that corresponds to an Arena with nRows rows and nCols columns. You may assume (i.e., you do not have to check) that it will be called with a first argument that does not exceed MAXROWS and a second that does not exceed MAXCOLS, and that neither argument will be less than 1.

The dropACrumb function is to be called to notify the Previous object that the player has arrived at or stayed at a grid point. The function returns false if row r, column c is not within bounds; otherwise, it returns true after recording what it needs to. This function expects its parameters to be expressed in the same coordinate system as the arena (e.g., row 1, column 1 is the upper-left-most position).

The showPreviousMoves function clears the screen and displays the grid of what has happened previously as the posted programs do. This function does clear the screen; it does not print the “Press Enter to continue” after the display.

The class declaration (with any private members you choose to add to support your implementation) must be in a file named Previous.h, and the implementation of the Previous class’s member functions must be in Previous.cpp. If you wish, you may add a public destructor to the Previous class. You must not add any other public members to the class. (This implies, for example, that you must not add a public default constructor.) The only member function of the Previous class that may cout is Previous::showPreviousMoves.

Add a data member of type Previous (not of type pointer-to-Previous) to the Arena class and provide this public function to access it; notice that it returns a reference to a Previous object.

class Arena {

<pre>       ...
       Previous&amp; thePrevious();
       ...
</pre>
};

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column"></div>
</div>
<div class="layoutArea">
<div class="column">
Have the player notify its arena’s Previous object about the player’s resulting position when the player stands or moves.

Have the Game recognize the new p command, tell the Arena’s Previous object to show the grid beforehand, and then print the “Press Enter to continue” prompt and wait for the user to respond. (cin.ignore(10000,’\n’); does that nicely.) Typing the p command does not count as the player’s turn.

Turn It In

By Thursday, July 2, there will be a link on CCLE that will enable you to turn in your source files. You do not have to turn in a report or other documentation for this project. What you will turn in for this project will be one zip file containing only the thirteen files you produced, no more and no less. The files must have these names exactly:

Robot.h Player.h Previous.h Arena.h Game.h globals.h Robot.cpp Player.cpp Previous.cpp Arena.cpp Game.cpp utilities.cpp main.cpp

The zip file itself may be named whatever you like.

If we take these thirteen source files, we must be able to successfully build an executable using g322 and one using either Visual C++ or clang++ — you must not introduce compilation or link errors.

If you do not follow the requirements in the above paragraphs, your score on this project will be zero. “Do you mean that if I do everything right except misspell a file name or include an extra file or leave off one semicolon, I’ll get no points whatsoever?” Yes. That seems harsh, but attention to detail is an important skill in this field. A draconian grading policy certainly encourages you to develop this skill.

The only exception to the requirement that the zip file contain exactly thirteen files of the indicated names is that if you create the zip file under Mac OS X, it is acceptable if it contains the additional files that the Mac OS X zip utility sometimes introduces: __MACOSX, .DS_Store, and names starting with ._ that contain your file names.

To not get a zero on this project, your program must meet these requirements as well:

Except to add the member function Arena::thePrevious() or to change string to std::string, you must not make any additions or changes to the public interface of any of the classes. (You are free to make changes to the private members and to the implementations of the member functions.) The word friend must not appear in any of the files you submit.

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>     #include "Game.h"
     #include "Game.h"
     #include "Arena.h"
     #include "Arena.h"
     #include "Previous.h"
     #include "Previous.h"
     #include "Player.h"
     #include "Player.h"
     #include "Robot.h"
     #include "Robot.h"
     #include "globals.h"
     #include "globals.h"
     int main()
</pre>
{}

If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>     #include "Previous.h"
     int main()
     {
</pre>
<pre>         Previous prev(2, 2);
         prev.dropACrumb(1, 1);
         prev.showPreviousMoves();
</pre>
}

Previous.h must not contain any #include line that, if removed, still allows the above replacement main.cpp to compile successfully under both g32 and either Visual C++ or clang++.

If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>     #include "Robot.h"
     int main()
     {
</pre>
<pre>         Robot r(0, 1, 1);
     }
</pre>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
Robot.h must not contain any #include line that, if removed, still allows the above replacement main.cpp to compile successfully under both g32 and either Visual C++ or clang++.

If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>     #include "Player.h"
     int main()
     {
</pre>
<pre>         Player p(0, 1, 1);
     }
</pre>
Player.h must not contain any #include line that, if removed, still allows the above replacement main.cpp to compile successfully under both g32 and either Visual C++ or clang++.

If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>     #include "Arena.h"
     int main()
     {
</pre>
<pre>         Arena a(10, 18);
</pre>
<pre>         a.addPlayer(2, 2);
     }
</pre>
Arena.h must not contain any #include line that, if removed, still allows the above replacement main.cpp to compile successfully under both g32 and either Visual C++ or clang++, except that Arena.h should include globals.h. (Even if Previous.h includes globals.h and Arena.h includes Previous.h, good practice says that the author of Arena.h who wants to use MAXROBOTS and knows that it’s declared in globals.h shouldn’t have to wonder whether some other header already includes globals.h.)

If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>     #include "globals.h"
     #include "Player.h"
     #include "Arena.h"
     int main()
</pre>
<pre>     {
         Arena a(10, 20);
         Player p(&amp;a, 2, 3);
</pre>
}

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>     #include "Arena.h"
     #include "Player.h"
     int main()
     {
</pre>
<pre>         Arena a(10, 20);
</pre>
<pre>         Player p(&amp;a, 2, 3);
     }
</pre>
If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>     #include "Player.h"
     #include "Arena.h"
     int main()
     {
</pre>
<pre>         Arena a(10, 20);
</pre>
<pre>         Player p(&amp;a, 2, 3);
     }
</pre>
If we replace your main.cpp file with the following, the program must build successfully under both g32 and either Visual C++ or clang++:

<pre>        #include "Arena.h"
        #include "Player.h"
        #include "Previous.h"
        #include "globals.h"
        int main()
</pre>
<pre>        {
            Arena a(2, 2);
</pre>
<pre>            a.addPlayer(1, 1);
            a.player()-&gt;move(RIGHT);
            a.player()-&gt;stand();
            a.player()-&gt;move(DOWN);
            a.thePrevious().showPreviousMoves();
</pre>
}

When executed, it must clear the screen (à la Arena::thePrevious), and write the following three lines (the third line is an empty line):

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
If we replace your main.cpp file with the following, the program must not build successfully; attempting to compile it should produce an error message like ‘r’ uses undefined class ‘Robot’ or Variable has incomplete type ‘Robot’ or variable ‘Robot r’ has initializer but incomplete type (and perhaps other error messages):

<pre>     #include "Player.h"
     #include "Arena.h"
     int main()
     {
</pre>
<pre>         Arena a(10, 20);
         Player p(&amp;a, 2, 3);
         Robot r(&amp;a, 1, 1);
</pre>
}

If we replace your main.cpp file with the following, the program must not build successfully; attempting to compile it should produce an error message like ‘a’ uses undefined class ‘Arena’ or Variable has incomplete type ‘Arena’ or variable ‘Arena a’ has initializer but incomplete type (and perhaps other error messages):

<pre>        #include "globals.h"
        #include "Robot.h"
        #include "Player.h"
        int main()
</pre>
<pre>        {
            Arena a(10, 10);
</pre>
}

If we replace your main.cpp file with the following, the program must not build successfully; attempting to compile it should produce an error message like ‘Previous’: no appropriate default constructor available or no matching constructor for initialization of ‘Previous’ or no matching function for call to Previous::Previous()’ (and perhaps other error messages):

<pre>     #include "Previous.h"
     int main()
     {
</pre>
<pre>         Previous prev;
     }
</pre>
If a .cpp file uses a class or function declared in a particular header file, then it should #include that header. The idea is that someone writing a .cpp file should not worry about which header files include other header files. For example, a .cpp file using an A object and a B object should include both A.h (where presumably the class A is declared) and

</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
<div class="layoutArea">
<div class="column">
B.h (where B is declared), without considering whether or not A.h includes B.h or vice versa.

To create a zip file on a SEASnet machine, you can select the thirteen files you want to turn in, right click, and select “Send To / Compressed (zipped) Folder”. Under Mac OS X, copy the files into a new folder, select the folder in Finder, and select File / Compress “folderName”; make sure you copied the files into the folder instead of creating aliases to the files.

Advice

Developing your solution incrementally will make your work easier. Start by making sure you can build and run the original program successfully with the one source file having the name main.cpp. Then, starting with Robot, say, produce Robot.h, removing the code declaring the Robot class from main.cpp, but leaving in main.cpp the implementation of the Robot member functions. Get that two-file solution to work. Also, make sure you meet those of the requirements above that involve only the Robot.h header.

Next, split off Player.h, testing the now three-file solution and also making sure you meet those of the requirements above that involve only the Robot.h and Player.h headers. Continue in this manner until you’ve produced all the required headers except Previous.h, the whole program still works, and you meet all the applicable requirements.

Now split off the member function implementations of, say, Robot, putting them in Robot.cpp. Test everything again. You see where this is going. The basic principle is to not try to produce all the files at once, because many misconceptions you have will affect many files. This will make it difficult to fix all those problems, since many of them will interfere with each other. By tackling one file at a time, and importantly, not proceeding to another until you’ve got everything so far working, you’ll keep the job manageable, increasing the likelihood of completing the project successfully and, as a nice bonus, reducing the amount of time you spend on it.

Help

While we will provide you assistance in clarifying what this assignment is asking for and in using g32 and either Visual C++ or clang++, we will otherwise offer minimal help with this assignment. This is to give you a chance to honestly evaluate your own current programming ability. If you find that you’re having trouble with the C++ program itself (not simply the Visual C++, Xcode, or g++ environment, which may be new to you), then you may want to reconsider your decision to take this class this quarter. Perhaps you’ve let your C++ programming skills get rusty, or maybe you didn’t learn the material in CS 31 or its equivalent very well. If you decide to take the course later, what you should do

</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="layoutArea">
<div class="column"></div>
</div>
<div class="layoutArea">
<div class="column">
between now and then is program, program, program! Solve some old or current CS 31 or PIC 10A or early PIC 10B projects, and read and do the exercises in a good introductory programming text using C++. You’ll have to be self-motivated to make time for that, but the payoff will be a greater likelihood for success in CS 32.

Endnotes

(1) “Correct” in terms of what a CS 31 student would know. For example, a CS 31 student wouldn’t know that sometimes you need to write a copy constructor, so the posted solution ignores that issue. (You don’t have to worry about that issue for this project, either.)

(2) As the Project Requirements document tells you, “build using g32” is shorthand for “build using g32 on lnxsrv07.seas.ucla.edu or lnxsrv09.seas.ucla.edu” — that specific command (g32, not g++) on one of those specific machines (not one of the other SEASnet Linux servers).

</div>
</div>
</div>
