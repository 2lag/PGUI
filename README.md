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

#BUTTON CLASS GOES DOWN HERE#
```

#### Preview
https://user-images.githubusercontent.com/96544487/194995938-dece5c83-a754-44b0-9169-317cf3b6eb39.mp4
