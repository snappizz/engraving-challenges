# LilyPond Engraving Challenge(s)

This document outlines the general rules that apply to our Engraving Challenges.
Please adhere to them as closely as possible, because otherwise the analysis of
the progress and the comparisons won't be reliable.

Let's start with a general 

#### "Code of Honor":

1. **Meticulously document progress**  
   We'll work inside a Git repository in order to have a full project history.
   For the purpose of our challenges it is important to make concise and
   fine-grained commits in order for the progress to be documented as detailed
   as possible. It may well be that this requires you to adopt a Git working style
   that is different from what you'd do on your own.   
   If you don't have experience with Git and aren't in the position to learn it
   for this occasion, don't worry. You can ask someone to assist you who will be
   able to commit your work as often as you think appropriate.
2. **Strictly follow the step-by-step rules of the challenge**  
   In order to be comparable and to allow us to make useful analysis it's important
   to do everything in a prescribed order. There are
   general rules **TODO: Add page and link to it**
   and possibly additional instructions specific to the given challenge.
3. **Be honest and transparent**  
   The main purpose of these challenges is to analyze the behaviour and performance
   of different notation programs when they are faced certain challenges.
   Although the comparison of different tools is an essential part of this project
   it's not the main goal, and it doesn't help anybody to play tricks.  
   While the text documents of tools like LilyPond can be easily tracked by Git
   this isn't the same with binary file formats. A LilyPond input file always reveals
   what is in it (what has been changed, what is default output) this isn't the same
   with other file formats. So - if you use programs with binary files - please be
   honest and document what you do as exactly as possible. Git's commit messages are
   a very suitable place for such documentation.
4. **Write reports about your experience**  
   We will provide pages on the Wiki for the documentation of each project.
   A home page for each challenge will provide specific information, and for each
   'competitor' there will be a dedicated page available.  
   The publication of the final analysis is intended on [Scores of Beauty]
   (http://lilypondblog.org), our LilyPond community blog.

#### Git Workflow

1. **Branches**  
   The `master` branch isn't intended for any work. All concrete work is done in
   feature branches that are merged into `master` only when a challenge or a
   significant task has been completed.  
   If in any doubt ask someone to set up a working branch for you.
2. **Merging into `master`**  
   Before a branch can be merged into `master` it has to be rebased to `master`.
   Then it has to be merged with an explicit merge commit with the `--no-ff`
   option.  
   If you don't consider yourself an administrator of this repository you should
   *not* merge the branch yourself but rather open a pull request.
3. **Commit strategies**  
   Please commit very often. We're particularly interested in the detailed
   documentation of the progress, therefore we need this information.  
   Use commit messages to leave as many information about what you did as possible.
   You can also use them to store timing information.  
   Please don't exceed 50 characters for the message header and 80 characters
   for the message body. Use hard line breaks and avoid whitespace at line ends.
4. **Tracking PDFs**  
   As a convenience we also track PDF files, which makes it easier to create a
   report of the progress. By default PDF files are ignored by the repository,
   so you should manually stage the PDF file to add it to the repository.
   However you should not commit *every* change of the PDF files but only
   relevant states (while you are encouraged to commit the changes to the
   document files as often as possible).