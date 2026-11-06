# Etch-a-Sketch TOP Project exercise by me

- Heavily based on [captainnairauk's Etch-a-Sketch project](https://github.com/captainnairauk/etch-a-sketch/tree/main) \
> the code for square opacity and RGB randomness was taken from his repo and modified to my liking

```html
function getRandomRGB() {
                const r = Math.floor(Math.random() * 256);
                const g = Math.floor(Math.random() * 256);
                const b = Math.floor(Math.random() * 256);
                return `rgb(${r}, ${g}, ${b})`;
            }

const randomColor = getRandomRGB();
      square.style.backgroundColor = randomColor;

      let currentOpacity = parseFloat(square.style.opacity);
      if (currentOpacity < 1) {
        square.style.opacity = (currentOpacity + 0.1).toString();
      }            
```
CSS taken from [MikeNewXYZ's Codepen project](https://codepen.io/MikeNewXYZ/pen/GRbedva) based on [this Reddit thread and answer](https://www.reddit.com/r/css/s/JXKDTQL98P) (found it myself ;) for a better layout solution and the `clientWidth` JS property for DOM manipulation in the script itself