http://bitbucketlabs.net/flashbake/

##flashbake
"This is the home page of the flashbake project, a seamless source control tool for ordinary people.  Automated backup is nice unless you have files for which you want to view an incremental history.  Source control is great for that history but most tools expect the author to manually commit their changes along the way.  A seamless source control solution combines the convenience of automated back up with the power of source version control.

For downloads and full documentation, go to the project page.

This software is still a bit rough (see the note below on the quick run up to the first public release).  If you have problems, feel free to contact me for help.  See the note under the Usage section about using the verbose switch; sending me verbose outputs along with an explanation of what you are trying will help figure out what is wrong faster."

##History

"This project was inspired by Cory Doctorow asking me for suggestions on source control for his writing and personal information files.  After a few rounds of correspondence, we realized that while source control was closer to what he needed than automated backup, it still wasn’t a perfect fit.  A little bit of research into seamless version control reveals some interesting research for ideas close to what he described but no actual code or code for much lower level projects, like file systems for viewing existing source control repositories or capturing versions without comment.

Cory wanted the version to carry prompts, snapshots of where he was at the time an automated commit occurred and what he was thinking.  I quickly sketched out a Python script to pull the contextual information he wanted and started hacking together a shell script to drive git, using the Python script’s output for the commit comment when a cron job invoked the shell wrapper.

I added my own idea to the project, borrowing from continuous integration build systems the idea of a quiet period.  I could easily imagine Cory actively working on a story, saving continually and a commit happening mechanically in the midst of that writing being less useful than if the script could find a quiet time to commit.  This enhancement prompted me to ditch my shell script wrapper and pull that logic all into Python.

I started the very first lines of code for this project on 1/25/2009 and on 2/12/2009 have a version I am ready to share."

