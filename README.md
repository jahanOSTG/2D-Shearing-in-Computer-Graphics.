# 2D Shearing in Computer Graphics

2D Shearing is a transformation technique used to change the shape of an object in a 2D plane by shifting points along the X or Y axis.

---

## Definitions

- Initial coordinates of a point: `(X_old, Y_old)`
- Shearing factor along X-axis: `Shx`
- Shearing factor along Y-axis: `Shy`
- New coordinates after shearing: `(X_new, Y_new)`

---

## Types of Shearing

### 1. Shearing in X Direction

- Equations:
  - `X_new = X_old + Shx * Y_old`
  - `Y_new = Y_old`

- Matrix form:
 <image src="s1.png" height="300" weight="300">


---

### 2. Shearing in Y Direction

- Equations:
- `X_new = X_old`
- `Y_new = Y_old + Shy * X_old`

- Matrix form:

 <image src="s2.png" height="300" weight="300">
---

## Algorithm Steps

1. **Input:** Point `(X_old, Y_old)` and shearing factors `Shx` and `Shy`.

2. **For Shearing in X direction:**
 - Calculate new X coordinate:  
   `X_new = X_old + Shx * Y_old`
 - Y coordinate remains the same:  
   `Y_new = Y_old`

3. **For Shearing in Y direction:**
 - X coordinate remains the same:  
   `X_new = X_old`
 - Calculate new Y coordinate:  
   `Y_new = Y_old + Shy * X_old`

4. **Output:** New point `(X_new, Y_new)` after shearing.

---

## Notes

- Shearing factors control the amount of slant.
- If `Shx` or `Shy` is zero, there is no shearing along that axis.
- The transformation preserves area but changes shape.
  
---

## Output Visualization: Shearing:
 <image src="s_output.png" height="500" weight="300">
