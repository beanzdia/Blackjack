**Note:** installation of programs and Git command lines may be different depending on your operating system, this user guide supplements a **Windows OS**.

To run this program, users should first have at least **Java JDK version 15.0.1** installed on their device; because this game was run with the most recent JDK version, prior versions will not allow our game to run. 

Users should also have their preferred development environment installed; our team mainly uses IntelliJ, however JGrasp works just as well. 

Once the correct version of JDK is installed or updated, users can then clone the Github repository to their computer, meaning they can make a copy of the online files and store them locally. To accomplish this, users must also have Git Bash installed. 

To clone a repository, open Git Bash, navigate to the folder you want to store our repository in(i.e. Documents), and type: 

`git clone https://github.com/beanzdia/test.git`
    
From there, our repository should be stored on your computer! You can then open your File Explorer, navigate to our ‘BlackJack’ repository, open the ‘src’ folder, open ‘BlackJack’ again, and from there, you should see our collection of .java files. 

Your folder tree should look something like:
> (ex.Documents) > BlackJack > src > BlackJack > ...

![alt](C:/Users/sakur/Downloads/folderTree.png)

Now, if you open **Main.java** in your dev environment, compile, and run it, a separate window with a green background and the title “BlackJack” across the top should appear. 

If not, here are some troubleshooting steps you can take:
- Make sure the JRE is running the latest version of Java version 15.0.1
- Make sure all of the files and dependencies are present i.e. all of the classes, the img folder, etc.

Once that window is up and running, you are now able to play a game of BlackJack! We will show more of the user flow in the video itself, but here are some of the main rules on how to play:
- Both the player(you) and the dealer(NPC) will have a hand of cards; the goal of BlackJack is to beat the dealer's hand without going over 21.
- Each player starts with two cards, and one of the dealer's cards is hidden until the end of the round.
- All face cards(Jack, Queen, King) are worth 10.
- To 'Hit' is to ask for another card. To 'Hold’' is to hold your total and end your turn. The player is able to keep hitting until they get a number that is close to or equals 21. The player may also hold their total and compare it to the dealer’s total at the end of the round.
- The player starts with $2500 in funds, and is able to make wagers each round they play by pressing the “bid” button. They can also double their bid when they have at least two cards in their hand.
#### Edge cases:
- When a player gets an Ace card, the player can choose a value of 1 or 11 for that card; the value is up to the discretion of the player.
- When a player acquires a double(e.g. A pair of Sevens), they can choose whether to split that hand or not. If accepted, the player will be able to split their one hand into two, meaning they have two hands to play with simultaneously. If one hand goes over 21, the player has another chance with the second hand. 