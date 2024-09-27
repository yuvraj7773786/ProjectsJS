# ProjectsJS :


## BackGround-Color-Changing

# Solution Code :
[Click Here](https://stackblitz.com/edit/stackblitz-starters-dpvuv4?file=1-ColourChange%2Findex.htm)

### Project 1


``` JavaScript
const button = document.querySelectorAll('.buttons');
const body = document.querySelector('body');

button.forEach(function (buttons) {
  console.log(buttons);
  buttons.addEventListener('click', function (e) {
    console.log(e);
    console.log(e.target);

    if (e.target.id === 'red') {
      body.style.backgroundColor = e.target.id;
    }
    if (e.target.id === 'yellow') {
      body.style.backgroundColor = e.target.id;
    }
    if (e.target.id === 'blue') {
      body.style.backgroundColor = e.target.id;
    }
    if (e.target.id === 'grey') {
      body.style.backgroundColor = e.target.id;
    }
  });
});
```
