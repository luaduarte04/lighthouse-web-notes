### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  hungry;
  availableTime;

  if (hungry === false) {
    console.log("I should get back at work.");
  }
  if (hungry) {
    if (availableTime < 20) {
      console.log("I have " + availableTime + " minutes. I should eat at the lab");
    } else if (availableTime >= 20 && availableTime <= 30) {
      console.log("I have " + availableTime + " minutes. I can go to a place near by for lunch.");
    } else if (availableTime > 30) {
      console.log("I have " + availableTime + " minutes. I should eat quick and go back at work, cause BOOTCAMP!");
    }
  }
};

whatToDoForLunch(true, 20);
console.log("---");

whatToDoForLunch(true, 50);
console.log("---");

whatToDoForLunch(false, 30);
console.log("---");

whatToDoForLunch(true, 15);
```