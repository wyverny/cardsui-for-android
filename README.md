CardsUI
===================
An open source library offering the popular Google Now & Google Play cards views

## Google Play Cards
This new type of card based on the new Google play design are highly customizable.

The parameters include :
* Title text (String)
* Description text (String)
* Title color (String)
* Stripe color (String)
* Menu overflow (Boolean)
* Touch feedback on click (Boolean)

Here is an example : 

    mCardView.addCard(new MyPlayCard(
            "Different Colors for Title & Stripe", 
            "You can set any color for the title and any other color for the left stripe", 
            "#f2a400", "#9d36d0", true, false));
            
            
## Additionnal Features
In addition to the Google Play cards, I made a few changes to the original library by [Nadav Fima](https://github.com/nadavfima/cardsui-for-android).

Those changes include :
*Ability to set regular cards's description text programmatically
Called like this :

    mCardView.addCard(new MyCard("title string", "description string");
    
*Ability to set stack titles's color programmatically
Called like this :

    CardStack stack = new CardStack();
    stack.setTitle("Card Title");
    stack.setColor("#33b5e5");
    mCardView.addStack(stack);
    
    
## CardsUI Generator
I'm working on a supplementary example app for the CardsUI library. This app includes a little daemon to generate cards and set their parameters with a nice animated gui.
Ultimately, the aim of this app will be to generate a zip file containing the code & resources needed for the cards "activity" the user generated in the app.
Considering that the cards layout needs to be on the app side, and not on the library side, this could be useful.

![screenshot1](http://imageshack.us/a/img837/1365/cardsgen1.png)![screenshot2](http://imageshack.us/a/img708/8929/cardsgen2.png)![screenshot3](http://imageshack.us/a/img90/7456/cardsgen3.png)![screenshot4](http://imageshack.us/a/img109/9287/cardsgen4.png)![screenshot5](http://imageshack.us/a/img209/8982/cardsgen5.png)![screenshot6](http://imageshack.us/a/img515/4987/cardsgen6.png)

