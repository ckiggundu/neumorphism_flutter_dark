
# Flutter: Neumorphism Modern UI (Dark Theme)

A flutter application to showcase how to create the Neumorphism effect.


## Deployment Setup

Clone the project

```bash
  git clone https://github.com/ckiggundu/neumorphism_flutter
```

Go to the project directory

```bash
  cd neumorphism_flutter_dark
```

Install dependencies

```bash
  flutter pub get
```

Start the device emulator

```bash
  flutter run
```


## Usage/Examples

```dart
return Scaffold(
    // make the background color grey
      backgroundColor: Colors.grey[850],

      // place everything in a body and center it
      body: Center(
          
          // create the container that holds the shape
        child: Container(

            //insert the image into the shape
          child: Image.asset(
            'images/icons8-instagram-250.png',
            height: 80,
            color: Colors.grey[700],
          ),
          padding: const EdgeInsets.all(30),

          //create the shape
          decoration: BoxDecoration(
            color: Colors.grey[850],

            // rectangle with rounded edges
            //borderRadius: BorderRadius.circular(12),

            shape: BoxShape.circle,

            // make list of box shadows to use more than one
            boxShadow: [
                
              //bottom right shadow is darker
              BoxShadow(
                color: Colors.grey.shade900,
                offset: const Offset(5, 5),
                blurRadius: 15,
                spreadRadius: 1,
              ),

              //top left shadow is lighter
              BoxShadow(
                color: Colors.grey.shade800,
                offset: Offset(-5, -5),
                blurRadius: 15,
                spreadRadius: 1,
              ),
            ],
          ),
        ),
      ),
    );
```

## Screenshots

[![Screenshot-2022-06-16-194828.png](https://i.postimg.cc/3wDBHx7j/Screenshot-2022-06-16-194828.png)](https://postimg.cc/p9R8fxmy)

