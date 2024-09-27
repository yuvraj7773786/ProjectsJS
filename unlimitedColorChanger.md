# ProjectsJS :


## Unlimited-BackGround-Color-Changer

# Solution Code :
[Click Here](https://stackblitz.com/edit/stackblitz-starters-kxq8iy?file=5-RandomColourGen%2Fgen.js)

### Project 5 : 


``` JavaScript
const randColor = function () {
  let color = '#';
  const hex = '0123456789ABCDEF';
  for (let i = 0; i < 6; i++) {
    color += hex[Math.floor(Math.random() * 16)];
  }
  return color;
};

let intervalID;
const startChangingColor = function () {
  if (!intervalID) {
    intervalID = setInterval(changeBgColor, 1000);
  }
  function changeBgColor() {
    document.body.style.backgroundColor = randColor();
  }
};

const stopChangingColor = function () {
  clearInterval(intervalID);
  intervalID = null;
};

document.querySelector('#start').addEventListener('click', startChangingColor);
document.querySelector('#stop').addEventListener('click', stopChangingColor);
```