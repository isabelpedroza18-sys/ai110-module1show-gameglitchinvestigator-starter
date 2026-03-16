# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it? a normal simple guessing game.
- List at least two concrete bugs you noticed at the start 
  (for example: "the hints were backwards").
  The hints were backwards. The answer was 69 and i typed 1. I was expecting "go higher", but instead it said "go lower".
  After a game ended, the message says "you won. the game has ended try starting a new game." Then, I pushed the new game or restart game button and the message would not dissapear.
  When on easy mode, I was supposed to guess from 1-20. I ran out of guesses and it said the correct answer was 98, which is definitely out of the range I was given to guess from.

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)? Copilot
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result). Flipping the output string for when guess < or > secret to match go lower or go higher appropriately.
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result). when fixing the backward hints it created an error message to appear, so copilot ran a test and had to edit some things to fix the issue it created.

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed? I had co pilot run some tests on test_game_logic.py and I re ran the app to test the fixes myself.
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code. I checked based on the secret number given, if i typed a number lower than that, it was supposed to give me a message to go higher and it did. It proved to me that the issue had been fixed on the code.
- Did AI help you design or understand any tests? How? It helped me design a test for the backward hints by creating and running a few test cases on the test_game_logic.py file.

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit? That we have to be careful on how the status is reset not just terminate it.

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects? being specific about the issue and wht the desired outcome should be when getting help from AI. Also, carefully go over the fixes that AI wants to implement before accepting the change.
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task? commiting my code before each AI edit to avoid big issues. 
- In one or two sentences, describe how this project changed the way you think about AI generated code. I can see how AI can help explain step by step logic or issues in my code.
