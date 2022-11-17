# Shopping Basket
## Proper Trench Coats
Trench coats are cool. Everyone should own a trench coat. The *“Proper Trench Coats”* store sells fashionable, elegant trench coats and the store needs software to allow their customers to order online. The application can be used in two modes: administrator and user. When the application is started, it will offer the option to choose the mode.

**Administrator mode:** The application has a database which holds available trench coats at a given moment. The store employees is able to update the database, meaning: add a new trench coat, delete a trench coat (when it is sold out) and update the information of a trench coat. Each **Trench Coat** has a `size`, a `colour`, a `price`, a `quantity` and a `photograph`. The photograph is memorised as a link towards an online resource (the photograph on the presentation site of the store). The administrators is also having the option to see all the trench coats in the store.

**User mode:** A user can access the application and choose one or more trench coats to buy. The application allows the user to:
- See the trench coats in the database, having a given size, one by one. If the size is empty, then all the trench coats will be considered. When the user chooses this option, the data of the first trench coat (size, colour, price, quantity) is displayed, along with its photograph.
- Choose to add the trench to the shopping basket. In this case, the price is added to the total sum the user has to pay. The total sum is being shown after each purchase.
- Choose not to add the trench coat to the basket and to continue to the next. In this case, the information corresponding to the next trench coat is shown and the user is again offered the possibility to buy it. This can continue as long as the user wants, as when arriving to the end of the list, if the user chooses next, the application will again show the first trench coat.
- See the shopping basket and the total price of the items.

## Requirements
**First Part**
This project has: 
- a graphical user interface using the Qt framework
- the interface design (location and size of GUI widgets, without attached functionalities), without using the Qt Designer
- the list or table displaying the repository entities in administrator mode are being populated using an input file
-	all functionalities are available through the GUI
- functionality of the application: including the one-by-one iteration of objects for the user mode

**Second Part**
1. Multiple *undo* and *redo* functionality for the `add`, `remove`, and `update` operations. I implement this functionality using inheritance and polymorphism. I also
have **Undo** and **Redo** buttons on the GUI, as well as a key combination to undo and redo the operations (e.g. `Ctrl+Z`, `Ctrl+Y`).

2. Show the contents of the `shopping basket` using a table view. I used the [Qt View/Model](https://doc.qt.io/qt-5/modelview.html) components (`QTableView`). I created my own model – a class which inherits from [`QAbstractTableModel`](https://doc.qt.io/qt-5/qabstracttablemodel.html). This window will be opened from GUI main window.
