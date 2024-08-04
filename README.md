# Completed-Prework

## WEB102 Prework - Sea Monster Crowdfunding

Submitted by: **Mohammed Fawzaan Khan**

**Sea Monster Crowdfunding** is a website for the company Sea Monster Crowdfunding that displays information about the games they have funded.

Time spent: **2** hours spent in total

## Required Features

The following **required** functionality is completed:

*  The introduction section explains the background of the company and how many games remain unfunded.
* The Stats section includes information about the total contributions and dollars raised as well as the top two most funded games.
*  The Our Games section initially displays all games funded by Sea Monster Crowdfunding.
* The Our Games section has three buttons that allow the user to display only unfunded games, only funded games, or all games.

## Video Walkthrough

Here's a walkthrough of implemented features:

https://imgur.com/KPxglxJ

GIF created with LICEcap then uploaded on imgur.com

## Notes

One challenge I encountered was setting up GitHub because my GitHub is registered under Mohammedkhan2619@gmail.com, while my computer is registered under fawzaan39khan@gmail.com, which took some time to resolve.

Apart from that, this prework was a good brush-up on JavaScript.

## Function Details

### `deleteChildElements(parent)`

This function removes all child elements from a given parent element. 
- **Input**: A parent HTML element.
- **Output**: The parent element will have no children.

**How it works**: 
1. It takes a parent element as an argument.
2. It keeps removing the first child of the parent until there are no more children left.

### `addGamesToPage(games)`

This function adds game cards to the web page.
- **Input**: An array of game objects.
- **Output**: Game cards are displayed on the page.

**How it works**:
1. It loops through each game in the array.
2. For each game, it creates a new `div` element.
3. It adds the class `game-card` to the `div` element.
4. It sets the inner HTML of the `div` to display the game's details (image, name, description, pledged amount, goal, and backers).
5. It appends the `div` element to the `gamesContainer` element on the page.

### `filterUnfundedOnly()`

This function filters and displays only the unfunded games.
- **Input**: None.
- **Output**: Unfunded game cards are displayed on the page.

**How it works**:
1. It calls `deleteChildElements` to remove all existing game cards.
2. It filters the `GAMES_JSON` array to get only the games that have not yet met their goal.
3. It calls `addGamesToPage` to display the filtered games.

### `filterFundedOnly()`

This function filters and displays only the funded games.
- **Input**: None.
- **Output**: Funded game cards are displayed on the page.

**How it works**:
1. It calls `deleteChildElements` to remove all existing game cards.
2. It filters the `GAMES_JSON` array to get only the games that have met or exceeded their goal.
3. It calls `addGamesToPage` to display the filtered games.

### `showAllGames()`

This function displays all games.
- **Input**: None.
- **Output**: All game cards are displayed on the page.

**How it works**:
1. It calls `deleteChildElements` to remove all existing game cards.
2. It calls `addGamesToPage` with the `GAMES_JSON` array to display all games.

## License

Copyright 2024 Fawzaan Khan

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
