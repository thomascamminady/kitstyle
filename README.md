# kitstyle
Use a nice KIT-ish theme for matplotlib plots.

## Install
place `kitish.mplstyle` in `~/.config/matplotlib/stylelib/`

## Usage
In Python, do
```python
import matplotlib.pyplot as plt
plt.style.use("kitish")

fig,ax = plt.subplots()
ax.plot([0,1,2],[1,2,1],label="cars")
ax.plot([0,1,2],[2,1,2],label="bikes")
ax.plot([0,1,2],[2,2,0],label="birds")
ax.plot([0,1,2],[0,1,1],label="cats")
plt.legend()
ax.set_title(r"Something $\alpha+\beta=\gamma$.")
ax.set_ylabel("Another label")
ax.set_xlabel(r"Source Sans Pro is a nice font.")
plt.savefig("example.png")
```
to get the following output:

![Alt text](/example.png?raw=true "Example plot")

For comparison, here's the original plot when omitting `plt.style.use("kitish")`.
![Alt text](/exampleold.png?raw=true "Standard example plot")


