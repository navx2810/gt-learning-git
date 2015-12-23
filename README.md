# How to does GitHub and Git

### Things you should know first
* Git and Github are the same as a folder existing on your desktop and the same folder sitting on your google drive. One's in the cloud, the other is on your computer.
* I'm going to update this repo with new information in order to explain commits. I'll be explaining commits while I commit commits. Meta as fuck.

## Wat is git?
Git is a source-control management solution. 

Git can be used as a *time-machine*. At any point, you can **commit** a snapshot of your project and then revert back to it later if you need or want too. Comparing it to a standard backup system would do it a disservice. With Git you can:

- Revert your project back to another commit
- Revert certain files back to another commit
- **Branch** your current commit, having a non-destructive way to add features
- Collaborate with others without passing around thumb-sticks
- Know exactly who to **blame** for fucking up your hard work by seeing their commit history 

Git isn't magic or time-lord science. It's more like a historian who will keep track of the **history** of your files. When you tell your historian to **commit** your files, they will record only the changes made compared to the previous commit. This is later explain in the *example* section.

Since Git keeps track of the history of the file, when you want to go back in time it literally recreates the file with the changes you made up to the point you want.

## Wat is GitHub?
Pretty much a cloud storage for your *repository*.

## Example in plain English
Okay I just created a word document listing all the good waifus. It's blank but I'll tell my historian: "I created this blank document and want you to note that I did". The historian then **commits** this to it's journal.

I then open up the document and begin by writing 

 - Rei (Evangelion)
 - Ryoko (Tenchi Muyo)
 - Faye (Cowboy Bebop)

I then wake up my historian and tell them: "I just added these three lines, write that down."
The historian will then write down that you added three lines consisting of "Rei, Ryoko and Faye".

Next I decide that I need to erase Rei from this list because I wish to trigger many animu fans. So I change the file.

- ~~Rei (Evangelion)~~
- Ryoko (Tenchi Muyo)
- Faye (Cowboy Bebop)

Again, I tell the historian: "I removed the first line".
The historian then looks back into it's journal and compares the past instructions to this one. It them writes in their journal that the first line was deleted.

Now I tell the historian I want to go back in time by one commit, The historian reads it's journal from the beginning and says that I created a blank document then I added three lines consisting of "Rei, Ryoko and Faye". 

At this point I redo my word document based on his instructions and get back to where I was one commit ago.

## How does this translate electronically?
First, I don't tell the historian what I did different, the historian figures out the differences (or **diffs**) themselves and commits them into it's journal. The only thing I really do is tell the historian which files to check the differences of and add a comment for each commit like "I added Hestia because she's the bestia" 

Check out the [commits](https://github.com/navx2810/gt-learning-git/commits/master) to this repository. You'll see that the first two commits are that I created the readme file and that I added this information to it. 

The third commit is this section. I obviously added this section, but I also removed the blank line under the **How does this translate electronically** header. You'll notice it has a - and + for line underneath the header. There is no move command, when you translate something up a line, It's really cut and pasted. This is actually two different instructions in the eyes of source control.

Commits are marked by +'s or -'s indicated if something was added or removed. 