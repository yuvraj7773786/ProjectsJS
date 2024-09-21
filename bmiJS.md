# Projects related to DOM

## projects links
[Click Here](https://stackblitz.com/edit/stackblitz-starters-vatw8b?file=2-BMI%2Fbmi.js)

## Solution Code

## project 2

```javascript
consoloe.log("Hi, Yuvraj...")

const form = document.querySelector('form');

form.addEventListener('submit', function (e) {
  e.preventDefault();
  const weight = parseInt(document.querySelector('#weight').value);
  const height = parseInt(document.querySelector('#height').value);
  const results = document.querySelector('.results');

  if (height === '' || height <= 0 || isNaN(height)) {
    results.innerHTML = `${height}, Invalid Height`;
  } else if (weight === '' || weight <= 0 || isNaN(weight)) {
    results.innerHTML = `${weight}, Invalid Weight`;
  } else {
    const bmi = (weight / ((height * height) / 10000)).toFixed(2);
    results.innerHTML = `<span>Your BMI is - ${bmi}</span>`;
  }
});
```