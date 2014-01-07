#### Git Workflow

This document describes the basic Git procedures for the "openLilyLib Engraving
Challenges" project.

---

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
