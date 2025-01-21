# PickledSnake game

This is a classic snake game written in *my* programming language [PickleLisp](https://github.com/Rad-hi/PickleLisp).

## Demo

<p align="center">
  <img src=".github/images/demo.gif">
</p>

## Run

```bash
cd PickledSnake
PickleLisp snake.pickle
```

## Reading the code

I realize that GitHub doesn't recognize the syntax, and neither would your text editor [probably].
I recommend enabling LISP mode and you'll get partial text highlighting (it really helps).

Here's a snippet from the `snake.pickle` script, when using Lisp mode, it's a bit better to read through:

```lisp
( if (food_exists)
    { nil }
    {
        ( DrawRectangle food_x food_y CELL_W CELL_H BG_COLOR )
        ( spawn_food {} )
        ( DrawRectangle food_x food_y CELL_W CELL_H FOOD_COLOR )
    }
)
```

## Why?

Because why not, and I wanted a goal to set for me to stop working on the language, and that goal was:
"Implement enough features to be able to load RayLib, and create a snake game with it."
