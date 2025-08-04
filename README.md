# Pokemon-Game
This project is a simple Pokemon Card Game inspired by the classic children's card game where two players draw a card, and the one with the higher experience wins.
Features & Requirements
Random Pokemon Selection
Each time the "Fight" button is clicked, both Player 1 and Player 2 are randomly assigned a Pokemon.

Experience-Based Winner
The Pokemon's experience (base_experience) is used to determine the winner of the round.

Score Tracking
The score of each player is displayed and incremented automatically based on who wins the round.

Player Containers
Each player has a dedicated container to display the selected Pokemon's:

Name

Image

Base Experience

Abilities

PokéAPI Integration
The application fetches data using the PokéAPI:

First, it retrieves a list of Pokemons.

Then, it selects one randomly for each player.

Finally, it fetches detailed data using the Pokemon-specific URL (e.g., experience, image, abilities).

Technical Workflow
Initialize Game State
On clicking the Fight button:

Fetch a list of Pokemons.

Randomly select one for each player.

Fetch Detailed Data
Use the url for each selected Pokemon to fetch its detailed data:

name

base_experience

sprites.front_default (image)

abilities

Render Pokemon Cards
Display the fetched details in each player’s container.

Determine Winner
Compare the base_experience of both Pokemons:

Increment the score of the player with higher experience.

Update the score display.

Tech Stack
HTML/CSS: For structure and styling

JavaScript: For DOM manipulation, API calls, and game logic

PokéAPI: Public API to get Pokemon data
