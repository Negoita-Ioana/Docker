<h1>Choose your Weapon: Rock, Paper, Scissors</h1>
<br />

From The Odin Project's <a href="http://www.theodinproject.com">Curriculum</a> <br /><br />


<img src="https://media.giphy.com/media/rfp9Znzj0NyWk/giphy.gif">

<h2>My Solution</h2>
<h3>Generate Random Computer Choice</h3>

```javascript
let computerSelection = () => {
  let randomCount = Math.random();

  if (randomCount < 0.34) {
    paraComputerResult.textContent = 'Computer selects rock';
    return 'rock';
  } else if (randomCount > 0.34 && randomCount < 0.68) {
    paraComputerResult.textContent = 'Computer selects paper';
    return 'paper';
  } else {
    paraComputerResult.textContent = 'Computer selects scissors';
    return 'scissors';
  }
}
```

<h3>Compare User and Computer choice</h3>

```javascript
let playRound = (playerSelection, computerSelection) => {
  if (playerSelection === computerSelection) {
    return 'It is a tie';
  } else if (playerSelection === 'rock' && computerSelection === 'paper') {
    return 'Computer wins!';
  } else if (playerSelection === 'rock' && computerSelection === 'scissors') {
    return 'You win!';
  } else if (playerSelection === 'paper' && computerSelection === 'rock') {
    return 'You win!';
  } else if (playerSelection === 'scissors' && computerSelection === 'rock') {
    return 'Computer wins!';
  } else if (playerSelection === 'scissors' && computerSelection === 'paper') {
    return 'You win!';
  } else if (playerSelection === 'paper' && computerSelection === 'scissors') {
    return 'You lose!';
  }
}
```

<h2>Demo</h2>
Link to Choose You Weapon Game --> <a href="https://ivanv257.github.io/Rock-Paper-Scissors-JavaScript-Project/">Play Now</a>





