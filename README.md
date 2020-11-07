# flutter_lab_4_1

A new Flutter project.

## #1 Animate a widget across screens

```flutter
import 'package:flutter/material.dart';

void animate() => runApp(HeroApp());

class HeroApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Transition Demo',
      home: MainScreen(),
    );
  }
}

class MainScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Main Screen'),
      ),
      body: GestureDetector(
        child: Hero(
          tag: 'imageHero',
          child: Image.network(
            'https://picsum.photos/250?image=9',
          ),
        ),
        onTap: () {
          Navigator.push(context, MaterialPageRoute(builder: (_) {
            return DetailScreen();
          }));
        },
      ),
    );
  }
}

class DetailScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: GestureDetector(
        child: Center(
          child: Hero(
            tag: 'imageHero',
            child: Image.network(
              'https://picsum.photos/250?image=9',
            ),
          ),
        ),
        onTap: () {
          Navigator.pop(context);
        },
      ),
    );
  }
}


```
![alt](https://picsum.photos/250?image=9)

## #2 Navigate to a new screen and back

```flutter


```
![alt](http://~)

## #3 Navigate with named routes

```flutter


```
![alt](http://~)

## #4 Pass arguments to a named route

```flutter


```
![alt](http://~)

## #5 Return data from a screen

```flutter


```
![alt](http://~)

## #6 Send data to a new screen

```flutter


```
![alt](http://~)