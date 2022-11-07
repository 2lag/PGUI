#### How to use
* Navigate to the [pgui_classes](https://github.com/2lag/PGUI/tree/main/pgui_classes) folder
* Open all folders of components you will need (or just grab from [here](https://github.com/2lag/PGUI/blob/faf12621cf59b16232a42c13ac15658781123f12/pgui_full/pgui_full.pde#L47) down in [pgui_full](https://github.com/2lag/PGUI/blob/main/pgui_full/pgui_full.pde)
* Copy the __entire__ class, everything AFTER the void setup(){} and void draw(){} functions.
* Create new components with the following syntax:

| Class | Arguments (In Order) |
| ----- | -------------------- |
| button | String txt, int xpos, int ypos, int buttonwidth |
| checkBox | int x, int y, int size, String text |
| comboBox | String[] list, int defaultselect, int xpos, int ypos |
| keyBind | String name, int xpos, int ypos |
| knob | int x, int y, int min, int max, int size, int scale |
| multiBox | String[] list, int xpos, int ypos |
| sliderInt | String name, int xpos, int ypos, float minimum, float maximum, float value, float size |
| textBox | int xpos, int ypos, int boxwidth |

#### Example Usage
```
button b = new button("test button: ", width / 2, height / 2, 0);

void setup() {
  size(400, 400);
}

void draw() {
  background(120);
  b.update();
}

*BUTTON CLASS HERE*
```

#### Preview
https://user-images.githubusercontent.com/96544487/194995938-dece5c83-a754-44b0-9169-317cf3b6eb39.mp4

#### BUGS🐛
I personally doubt anybody will use this, but in the case that you ARE actually using this for something, and you run across a mischevious bug, feel free to submit an issue if you don't know how to fix it, and I'll tinker around until it's fixed, then push a new update and let you know in your original post before I mark it as completed. If you DO know how to fix it, please consider contributing to this project as I'd love to see what features/fixes we could potentially add in the future!
