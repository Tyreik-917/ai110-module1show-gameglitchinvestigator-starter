# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
  
  Loading up the page I realized that the range of numbers a user can guess from under "Make a guess" remade the same even after changing the diffculty where each difficulty has its own range of numbers to guess from. After I started gussing numbers and even guessed numbers outside the provided range, letters, and empty inputs (example: "") and the game continued and counted it as a attempt. Some other bugs I found were whenever I start a new game it would still have infomation in the "Developer Debug info" section. Finally I tried entering guesses and after reaching the max number of attempts the game still continued.

**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
|   0   | Attempts left: 3    Attempts left: 2    Invaild input
|       | (remains the same)
|       |
|   0   | Not within range    Go higher/lower   Out of range error
|       |
|   1w  | invalid input       counted as a attempt   
|   


---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

Used it to identify and the fix the bugs after telling it what the bugs were and then came up with test cases to test the code
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?
I asked for possible test cases I can try on the app and then tested them to see if the app worked as expected (Ex: entered 1w as an input and then the app didnt count it as a valid input and didnt decrease my attempts).
---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
A script running from top to bottum whenever you click a button
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
