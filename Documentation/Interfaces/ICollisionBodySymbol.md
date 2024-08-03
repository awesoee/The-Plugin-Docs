This is an extension of [IBaseSymbol](/Documentation/Interfaces/IBaseSymbol.md) and [IColorableSymbol](/Documentation/Interfaces/IColorableSymbol.md).

## Properties

| Prop Name | Value | Description |
| --------------------- | ------ | ------------------- |
| type | `'COLLISION_BODY'` | ![image](https://github.com/user-attachments/assets/5164362e-2c84-4e24-a26a-ddf153909dd7) |
| head | number | Y coordinate of topmost point of the collision body |
| foot | number | Y coordinate of bottommost point of the collision body|
| hipWidth | number | Amount of X units between leftmost point and rightmost point |
| hipXOffset | number | Amount of X units the hip's midpoint is offset from the midpoint of the head and foot. <br/> Positive = to the right, Negative = to the left |
| hipYOffset | number | Amount of Y units the hip's midpoint is offset from the midpoint of the head and foot. <br/> Positive = closer to the feet, Negative = closer to the head|
