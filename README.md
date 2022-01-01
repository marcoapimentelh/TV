# TV

import 'package:flutter/material.dart';
const _backgroundColor = Color (0XFFF6F5F2);
class GroceryStoreHome extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Column(
        children: [
          _AppBarGrocery(),
        ],
      ), //Column
    ); //Scaffold
  }
}

class _AppBarGrocery extends StateleesWidget {
  @override
  Widget build(BuildContext context) {
    return Container(
            height: kToolbarHeight,
            color: _backgroundColor
            child: Row(
              children: [
                BackButton(
                  color: Colors.black,
                ), //BackButton
                const SizedBox(width: 10),
                Expanded(
                  child: Text(
                    'Farmacia',
                    style: Textstyle(
                      color: Colors.black,
                ), // Expanded
                IconButton(
                  icon: Icon(
                    Icons.settings,
                  ), //Icon
                  onPressed: () => null,
                ), //IconButton
              ],
            ), //Row
          ), //Container
  }
}


  
  
