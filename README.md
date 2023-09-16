import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: ShoppingListApp(),
    );
  }
}

class ShoppingListApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('My Shopping List'),
        actions: [
          IconButton(
            icon: Icon(Icons.shopping_cart),
            onPressed: () {
              // Implement cart functionality here
            },
          ),
        ],
      ),
      body: ListView(
        children: [
          ListTile(
            leading: Icon(Icons.shopping_basket),
            title: Text('Apples'),
          ),
          ListTile(
            leading: Icon(Icons.shopping_basket),
            title: Text('Bananas'),
          ),
          ListTile(
            leading: Icon(Icons.shopping_basket),
            title: Text('Bread'),
          ),
          ListTile(
            leading: Icon(Icons.shopping_basket),
            title: Text('Milk'),
          ),
          ListTile(
            leading: Icon(Icons.shopping_basket),
            title: Text('Eggs'),
          ),
          // Add more shopping items here
        ],
      ),
    );
  }
}

