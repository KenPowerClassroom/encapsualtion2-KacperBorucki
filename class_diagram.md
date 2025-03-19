```mermaid
classDiagram

    class Square {
        float size
        +area()::float
    }

    class Circle {
        radius:float
    }

    class Figure {
        
    }

    class KacperBorucki {

    }

   class Shape {
        draw(win:Window)
        rotate(angle:float)
   }
    <<interface>> Shape 

    Figure o-- Shape : is made up of

    Shape .. KacperBorucki
    Shape <|.. Square
    Shape <|.. Circle

    class Window {

    }

    class Color {
        -r:int
        -g:int
        -b:int
    }

KacperBorucki -- Window
Shape <.. Window
Shape *-- Color

   

    
