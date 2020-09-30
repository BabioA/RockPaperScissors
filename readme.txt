// Rock paper scissors

i want to add the random computerPlay to the html field
not yet the playerselection input

the function should be called and then returned with one of the 3 options
i just added () and everything was fixed lol 

(3) 

// options = ["rock", "paper", "scissors"]

// function = computerPlay() {
//	let index = Math.floor(Math.random() * 3);
//	return options[index];
// }


(4) function that plays a single game of rps

playerselection = window.prompt('Input to play rock, paper & scissors', 'rock');

function round(playerselection, computerselection) {
	// do the lets go here?
	if ((playerselection === "rock" && computerselection === "scissors") || (playerselection === "paper" && computerselection === "rock") || 
		(playerselection === "scissors" && computerselection === "paper")) {
		playerScore = playerScore + 1
		message("Won",playerselection,computerselection)
		
	} else if { (playerselection === computerselection)
		message("Tied",computerselection,playerselection)

	} else {
		computerScore = computerScore + 1
		message("lost",computerselection,playerselection)
	}
}
/////


(4/1)prompt/input("choose rock paper or scissors")  (/i)

make a const for every posible option of writting of rps (in input):

const patterns = {
    rock: /^rock$/i,
    paper: /^paper$/i,
    scissors: /^scissors$/i;
}

make a function to validate if the inputed text matches any of the patterns

function validate(field, regex){
    if(regex.test(field.value)){
        field.className = 'valid';
    } else {
        field.className = 'invalid';
		// alert("you have entered a bad value")
    }
}

if it matches the text is valid and it should procede with the code
if it doesnt match the text is unvalid and an alert should popup

the input might be case insensitive but not the === in the round function
so what may happen is that the alert pops up if the input != one of the options
but it goes to the else part because "rock" isn't defined case-sensitive there


it should be noted that computerPlay isn't case sensitive because it picks one of the values of the array


/////



(5) 

function message(result, winningvalue, losingvalue) {
	return "You " + result + " ! " + winningvalue + " beat " losingvalue;
}


(6)
playerScore = 0
computerScore = 0

playerScore = playerScore + parseInt(1)
computerScore = computerScore + parseInt(1)

the winner of the 5 rounds wins a game
function game{ 
	console.log(round(playerselection,computerselection));
	console.log(round(playerselection,computerselection));
	console.log(round(playerselection,computerselection));
	console.log(round(playerselection,computerselection));
	console.log(round(playerselection,computerselection));
}

function caclScore(playerScore,computerScore){
	if (playerScore > computerScore) {
		return finalmessage("won",playerScore,computerScore);
	} else if (playerScore === computerScore) {
		return finalmessage("tied",playerScore,computerScore);
	} else {
		return finalmessage("lost",computerScore,playerScore + " better luck next time!");
	}
}

resultGame =! result because result is of every round and not the 5 ones in a game

function finalmessage(resultGame,playerScore,computerScore){
	return("You " + resultGame + " the game, you scored " + playerScore + " and the computer scored " + computerScore);
}


return caclScore(playerScore,computerScore)

<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
        <script>
            
        </script>
    </body>
</html>


            function caclScore(playerScore,computerScore){
	            if (playerScore > computerScore) {
		            return finalmessage("won",playerScore,computerScore);
	            } else if (playerScore === computerScore) {
		            return finalmessage("tied",playerScore,computerScore);
	            } else {
	            	return finalmessage("lost",playerScore,computerScore + " better luck next time!");
	            }
            }

            function finalmessage(resultGame,playerScore,computerScore){
	            return("You " + resultGame + " the game, you scored " + playerScore + " and the computer scored " + computerScore);
            }

            alert(caclScore(playerScore,computerScore));