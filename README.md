# Playlist Chaos

Your AI assistant tried to build a smart playlist generator. The app runs, but some of the behavior is unpredictable. Your task is to explore the app, investigate the code, and use an AI assistant to debug and improve it.

This activity is your first chance to practice AI-assisted debugging on a codebase that is slightly messy, slightly mysterious, and intentionally imperfect.

You do not need to understand everything at once. Approach the app as a curious investigator, work with an AI assistant to explain what you find, and make targeted improvements.

---

## How the code is organized

### `app.py`  

The Streamlit user interface. It handles things like:

- Showing and updating the mood profile  
- Adding songs  
- Displaying playlists  
- Lucky pick  
- Stats and history

### `playlist_logic.py`  

The logic behind the app, including:

- Normalizing and classifying songs  
- Building playlists  
- Merging playlist data  
- Searching  
- Computing statistics  
- Lucky pick mechanics

You will need to look at both files to understand how the app behaves.

---

## What you will do

### 1. Explore the app  

Run the app and try things out:

- Add several songs with different titles, artists, genres, and energy levels  
- Change the mood profile  
- Use the search box  
- Try the lucky pick  
- Inspect the playlist tabs and stats  
- Look at the history  

As you explore, write down at least five things that feel confusing, inconsistent, or strange. These might be bugs, quirks, or unexpected design decisions.

### 2. Ask AI for help understanding the code  

Pick one issue from your list. Use an AI coding assistant to:

- Explain the relevant code sections  
- Walk through what the code is supposed to do  
- Suggest reasons the behavior might not match expectations  

For example:

> "Here is the function that classifies songs. The app is mislabeling some songs. Help me understand what the function is doing and where the logic might need adjustment."

Before making changes, summarize in your own words what you think is happening.

### 3. Fix at least four issues  

Make improvements based on your investigation.

For each fix:

- Identify the source of the issue  
- Decide whether to accept or adjust the AI assistant's suggestions  
- Update the code  
- Add a short comment describing the fix  

Your fixes may involve logic, calculations, search behavior, playlist grouping, lucky pick behavior, or anything else you discover.

### 4. Test your changes  

After each fix, try interacting with the app again:

- Add new songs  
- Change the profile  
- Try search and stats  
- Check whether playlists behave more consistently  

Confirm that the behavior matches your expectations.

### 5. Optional stretch goals  

If you finish early or want an extra challenge, try one of these:

- Improve search behavior  
- Add a "Recently added" view  
- Add sorting controls  
- Improve how Mixed songs are handled  
- Add new features to the history view  
- Introduce better error handling for empty playlists  
- Add a new playlist category of your own design  

---

## Tips for success

- You do not need to solve everything. Focus on exploring and learning.  
- When confused, ask an AI assistant to explain the code or summarize behavior.  
- Test the app often. Small experiments reveal useful clues.  
- Treat surprising behavior as something worth investigating.  
- Stay curious. The unpredictability is intentional and part of the experience.

When you finish, Playlist Chaos will feel more predictable, and you will have taken your first steps into AI-assisted debugging.

### Summary : Debugging with AI in Playlist Chaos

# Overview

The core overview of this activity was understanding how application state and logic flow across multiple files. Features like playlist assignment, search, Lucky Pick, and statistics all depend on shared data structures and conditional logic. Students needed to recognize how a single user interaction in the Streamlit interface connects to functions in playlist_logic.py, and how small logic decisions can directly impact visible behavior in the app.

# Where Students Are Most Likely to Struggle

Students are most likely to struggle with tracing how data moves through the app and identifying where state is updated or misused. It can be difficult to connect unexpected UI behavior to a specific conditional statement or list mutation in another file. Issues like mmisplaced if/elif branches can make a small bug feel much more complex than it actually is.

# Where AI Was Helpful vs. Misleading

AI was especially helpful when explaining what a highlighted block of code was doing such as how lists were being modified. It worked best when used to understand behavior before attempting changes. However, it could be misleading when it confidently suggested large refactors or fixes that changed more logic than intended or did not fully match what was happening in the running app. Treating AI responses as hypotheses rather than final answers was essential.

# How I Would Guide a Student Without Giving the Answer

Instead of giving the solution, I would ask the student to clearly state one specific expectation and then trace where that value is created, checked, and updated in the code. I would prompt them to compare their mental model of the rule to the actual conditionals and state updates in the program. This approach helps them identify mismatches independently while strengthening their debugging skills before checking with AI.