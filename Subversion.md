Page about problems/information related to Subversion.

A notable tool in conjunction with using NetBeans' plugin for Subversion, there is also TortoiseSVN which is a graphical UI for SVN instead of the regular console command line way. I personally use TortoiseSVN to explore the repository and delete files and edit their titles when necessary (Eric).

Commits:

After attempting to commit after generating Javadocs in NetBeans results in getting an error along the lines of "already under version control".

If the directory in question is the doc folder, then when trying to make a commit, deselect the doc folder. I'm not too sure why this problem happens. Hopefully we can eventually figured it out...

Updating:

For some reason, when updating a project, if new files were added (new classes/packages) then updates sometimes don't pick up on those. In this case, you can delete the project you're working with (make a backup first) and then do a Subversion checkout operation.