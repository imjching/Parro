# Parro

A technical interviewing platform capable of asking both behavioral and technical questions and analyzing a candidate's performance intelligently.

## Table of Contents

- [Project Overview](#project-overview)
- [Demo](#demo)
- [Contributing](#contributing)

## Project Overview

This was an idea that resulted from a number of pivots before we ultimately zeroed in on exactly the problem we wanted
to solve: a technical interview process that's automated from start to finish. We've even added support for a Q&A session at the end of the interview, where candidates can ask Parro about the company for which they're interviewing and receive answers. There are platforms that handle the technical side like HackerRank, Codility, and others, but none of them provide support for automating the behavioral side of the hiring process, which really matters to certain startups and companies. That's what Parro was built to do.

**Behavioral Implementation**
--facial recognition and login

For the behavioral interview, we used IBM Watson to perform speech to text translation, tone analysis, personality insight, and text to speech conversion. This allowed us write algorithms to pull metrics out of a candidate's responses like their most frequently used words, use of hesitation words (use of "like", "um", and "uh", for example), speech clarity and coherence, and speaking speed.

**Technical Implementation**

For the technical interview, we used the [React version](https://github.com/JedWatson/react-codemirror) of CodeMirror to embed a Text Editor into a webpage. Since there's no way to run code inside of that editor, we had to pull the code out of the text editor and make a request to the backend. From there, we used [glot.io](http://glot.io/) to actually run the candidate's code using test inputs. Depending on whether their output was correct, incorrect, or errored, we sent a response back to the frontend that rendered a message with the result.

**Q&A**


**Statistics**

## Demo


## Contributing

Interested in contributing to this project? Feel free! Create a branch, add commits, and [open a pull request](https://github.com/benhubsch/Parro/compare/).