# Projects related to DOM

## projects links
[Click Here](https://stackblitz.com/edit/stackblitz-starters-rqb9ij?file=3-DigitalClock%2Fclock.js)

## Solution Code

## project 3

```javascript
consoloe.log("Hi, Yuvraj...")
const clock = document.querySelector('.clock');

setInterval(function () {
  let date = new Date();
  clock.innerHTML = date.toLocaleTimeString();
}, 1000);
```