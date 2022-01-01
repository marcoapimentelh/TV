# TV

import 'package:flutter/material.dart';
const _backgroundColor = Color (0XFFF6F5F2);
const _cartBarHeight = 100.0;

class GroceryStoreHome extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Column(
        children: [
          _AppBarGrocery(),
          Expanded(
            child: Stack{
              children: [
                Positioned{
                  left: 0,
                  right: 0,
                  top: -_cartBarHeight,
                  height: size.height - kToolbarHeight,
                  child: Container(
                    decoration: BoxDecoration(
                      color: Colors.white, 
                      borderRadius: BorderRadius.only(
                        bottomLeft: Radius.circular(
                          30,
                        ), // Radius.circular
                        bottomRight: Radius.circular(
                          30,
                     
                        ), //Radius.circular
                      ), //BorderRadius.only
                    ), //BoxDecoration
                  ), //Container
                ), //Positioned
                Positioned{
                  left: 0,
                  right: 0,
                  top: size.height - kToolbarHeight - _cartBarHeight ,
                  height: size.height,
                  child: Container(
                    color: Coolors.black,
                  ), //Container
                ), //Positioned
              ],
            ), // Stack
          ), // Expanded
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


  
  
