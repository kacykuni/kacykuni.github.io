---
layout: project
type: project
image: img/istockphoto-1206806317-612x612.jpg
title: "Shopping Cart GUI"
date: 2023
published: true
labels:
  - Java
  - ICS 111
  - IntelliJ IDE
summary: "One of my final projects in ICS 111 and my first time using GUI in Java"
---

![Screenshot 2025-09-11 184100](https://github.com/user-attachments/assets/68bfa827-6675-4719-b56a-fc3362b797de)


For this final project in my ICS 111 class we were tasked to create a shopping cart application with a graphical user interface using Java Swing. This program allowed users to add items from a fixed drop down list of catagories and items, add different quantities, view their cart, and calculate their total with tax included.
This was my first time working with GUI programming, it was very interesting and fun to be able to play with the different components like JFrame, JPanel, JList, and JOptionPane to create small or big interactive windows and buttons. This was a huge shift than working with user input and arguments. 
Overall, the project gave me a basic understanding of how GUIs are build and how complex coding must be on a larger scale with applications that I use everyday. It was definitely a challenging project for someone like me as a beginner programmer at the time, but it showed me how programming can create real and interactive applications. 

Here is some code that illustrates how I used graphical user interface in my programming:

```cpp
    public ShoppingCartGUI() {
        setTitle("Shopping Cart");
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLayout(new BorderLayout());

        // Create a DefaultListModel and JList
        listModel = new DefaultListModel<>();
        itemList = new JList<>(listModel);

        // Create JScrollPane to hold the JList
        JScrollPane scrollPane = new JScrollPane(itemList);
        add(scrollPane, BorderLayout.CENTER);

        JPanel topPanel = new JPanel(new BorderLayout());

        shoppingCart = new ShoppingCart(listModel);

        // Create buttons for manipulating the list
        JButton addButton = new JButton("Add Item");
        JButton checkoutButton = new JButton("Checkout");

        // Add action listeners to the buttons
        addButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                addItem();
            }
        });

        checkoutButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                checkout();
            }
        });

        // Create a panel for the buttons
        JPanel buttonPanel = new JPanel();
        buttonPanel.add(addButton);
        buttonPanel.add(checkoutButton);

        // Add the button panel to the frame
        topPanel.add(buttonPanel, BorderLayout.NORTH);

        totalItemsLabel = new JLabel("Total Items: 0");
        topPanel.add(totalItemsLabel, BorderLayout.CENTER);

        add(topPanel, BorderLayout.NORTH);

        subtotalLabel = new JLabel("Subtotal: $0.00");
        add(subtotalLabel, BorderLayout.SOUTH);

        itemQuantities = new HashMap<>();

        // Set frame size and make it visible
        setSize(300, 200);
        setLocationRelativeTo(null);
        setVisible(true);
    }
```
