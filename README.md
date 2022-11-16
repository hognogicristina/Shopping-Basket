# Shopping Basket
## Proper Trench Coats
Trench coats are cool. Everyone should own a trench coat. The *“Proper Trench Coats”* store sells fashionable, elegant trench coats and the store needs software to allow their customers to order online. The application can be used in two modes: administrator and user. When the application is started, it will offer the option to choose the mode.\

**Administrator mode:** The application will have a database which holds available trench coats at a given moment. The store employees must be able to update the database, meaning: add a new trench coat, delete a trench coat (when it is sold out) and update the information of a trench coat. Each **Trench Coat** has a `size`, a `colour`, a `price`, a `quantity` and a `photograph`. The photograph is memorised as a link towards an online resource (the photograph on the presentation site of the store). The administrators will also have the option to see all the trench coats in the store.\

**User mode:** A user can access the application and choose one or more trench coats to buy. The application will allow the user to:
- See the trench coats in the database, having a given size, one by one. If the size is empty, then all the trench coats will be considered. When the user chooses this option, the data of the first trench coat (size, colour, price, quantity) is displayed, along with its photograph.
- Choose to add the trench to the shopping basket. In this case, the price is added to the total sum the user has to pay. The total sum will be shown after each purchase.
- Choose not to add the trench coat to the basket and to continue to the next. In this case, the information corresponding to the next trench coat is shown and the user is again offered the possibility to buy it. This can continue as long as the user wants, as when arriving to the end of the list, if the user chooses next, the application will again show the first trench coat.
- See the shopping basket and the total price of the items.

## Requirements
**First Part**
- Create a graphical user interface using the Qt framework for the problem you have been working on.

- Implement the interface design (location and size of GUI widgets, without attached functionalities), without using the Qt Designer
- The list or table displaying the repository entities in administrator mode should be populated using an input file. 

-	All functionalities must be available through the GUI

**Second Part**
- Create a graphical user interface using the Qt framework for the problem you have been working on.

- Implement the interface design (location and size of GUI widgets, without attached functionalities), without using the Qt Designer.
- The list or table displaying the repository entities in administrator mode should be populated using an input file.

-	All functionalities must be available through the GUI. You may use Qt Designer, if you want to change the initial design of your GUI.
-	The functionality of the application must be the same (including the one-by-one iteration of objects for the user mode).

**Third part**
1. Add multiple *undo* and *redo* functionality for the `add`, `remove`, and `update` operations. Implement this functionality using inheritance and polymorphism. You will have **Undo** and **Redo** buttons on the GUI, as well as a key combination to undo and redo the operations (e.g. `Ctrl+Z`, `Ctrl+Y`).

2. Show the contents of the `adoption list` / `movie watch list` / `shopping basket` / `tutorial watch list` using a table view. You must use the [Qt View/Model](https://doc.qt.io/qt-5/modelview.html) components (`QTableView`). Create your own model – a class which inherits from [`QAbstractTableModel`](https://doc.qt.io/qt-5/qabstracttablemodel.html). This window will be opened from your GUI main window.
