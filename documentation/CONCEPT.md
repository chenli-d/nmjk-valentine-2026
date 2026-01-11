Project Concept & Technical Plan (Draft) 0. Deployment & Play Experience

0.1 This project is a web-based Visual Novel (VN), designed to be playable directly in a mobile browser.
0.2 Players are not required to download or install any software; the game can be played by simply opening a web link.
0.3 Players access and continue their progress using a unique access code.

1. Creative & Production Workflow

1.1 The project prioritizes narrative design and writing above all else.
1.2 During the initial phase, Twine will be used to complete the hookup tasks:
a. Writing story text
b. Designing multi-branch narrative structures
c. Implementing variables and conditional logic (for route branching and cross-route influence)
1.3 If time and resources allow, once the narrative structure is finalized, the content may be migrated to RenJS or Monogatari in order to:
a. Manage UI, character sprites, backgrounds, and audio in a unified way
b. Present game states and save data more clearly
1.4 If the development timeline is constrained, the Twine version may be released as the final version of the game.

2. Game Type & Core Gameplay

2.1 The game is classified as a Visual Novel (VN).
2.2 Gameplay is primarily reading-focused, with player choices serving a secondary but critical role.
2.3 Players make decisions at key narrative moments, which lead to different story routes.
2.4 The game emphasizes a comparative multi-route experience, encouraging replay to understand how different choices result in different outcomes.

3. Narrative Structure

3.1 The game consists of three primary story routes.
3.2 A full understanding of the story requires completing all three routes.
3.3 The routes are not completely independent:
a. Key choices made in one route
b. May affect dialogue, story details, or available information in later routes
3.4 Cross-route effects are recorded using global state flags.

4. Player Identity & Save System

4.1 The project does not use a traditional account or password-based system.
4.2 Players are identified using a unique access code issued by the creator.
4.3 The access code is used to:
a. Identify the player
b. Bind their progress and recorded choices
4.4 Players may set a custom display name, which is used only for narrative or UI presentation purposes.

5. Data Storage & Technical Implementation

5.1 Supabase is used as the backend data storage service.
5.2 Stored data includes:
a. Player identity records associated with access codes
b. Progress data for each story route
c. Player choices made at key narrative points
d. Global state data used for cross-route influence
5.3 The save system prioritizes stability and low maintenance cost over high-level security.

6. Project Scope & Design Philosophy

6.1 This is a small-scale fan project, with a limited expected player base.
6.2 Technical decisions are made to serve narrative completeness, avoiding unnecessary system complexity.
6.3 All technology choices are guided by the principle of not interfering with the writing process.
