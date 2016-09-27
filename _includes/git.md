<pre><code>git init
git remote add origin [eigen link]
git fetch
git checkout [branch]
git add --all
git commit -m "comment"
git push origin [branch]</code></pre>
<h4>Or create a new respository from the command line</h4>
<pre><code>echo "# [repo name]" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:[alias]/[branch].git
git push -u origin master</code></pre>
<h4>Or push an existing repository from the command line</h4>
<pre><code>git remote add origin git@github.com:[alias]/[branch].git
git push -u origin master</code></pre>
<h3>Setup</h3>
<h4>Configuring user information used across all local repositories</h4>
<table>
	<tbody>
		<tr>
			<td>git config --global user.name "firstname lastname"</td><td>Set a aname that is identifiable for credit when reviewing version history</td>
		</tr>
		<tr>
			<td>git config --global user.email "email"</td><td>Set an email address that will be associated with each history marker</td>
		</tr>
		<tr>
			<td>git config --global color.ui auto</td><td>Set automatic command line coloring for Git for easy reviewing</td>
		</tr>
	</tbody>
</table>
<h3>Init</h3>
<h4>Initializing and cloning repositories</h4>
<table>
	<tbody>
		<tr>
			<td>git init</td><td>Initialize an existing direcotry</td>
		</tr>
		<tr>
			<td>git clone url</td><td>Retrieve an entire repository from a hosted location via <em>url</em></td>
		</tr>
	</tbody>
</table>
<h3>Stage & Snapshot</h3>
<h4>Working with snapshots and the Git staging area</h4>
<table>
	<tbody>
		<tr>
			<td>git status</td><td>Show modified files in working directory, staged for your next commit</td>
		</tr>
		<tr>
			<td>git add [file]</td><td>Add <em>file</em> as it looks now to your next commit (stage)</td>
		</tr>
		<tr>
			<td>git reset [file]</td><td>Unstage <em>file</em> while retaining the changes in working directory</td>
		</tr>
		<tr>
			<td>git diff</td><td>Show a diff of what is changed but not staged</td>
		</tr>
		<tr>
			<td>git diff --staged</td><td>Show a diff of what is staged but not yet committed</td>
		</tr>
		<tr>
			<td>git commit -m "descriptive message"</td><td>Commit your staged content as a new commit</td>
		</tr>
	</tbody>
</table>
<h3>Branch & Merge</h3>
<h4>Isolating work in branches, changing context and integrating changes</h4>
<table>
	<tbody>
		<tr>
			<td>git branch</td><td>List your branches. A * will appear next to the currently active branch</td>
		</tr>
		<tr>
			<td>git branch [branch-name]</td><td>Create a new branch with name <em>branch-name</em> at the current commit</td>
		</tr>
		<tr>
			<td>git checkout</td><td>Switch to another branch and check it out into your working directory</td>
		</tr>
		<tr>
			<td>git merge [branch]</td><td>Merge the history of branch with name <em>branch</em> into the current one</td>
		</tr>
		<tr>
			<td>git log</td><td>Show all commits in the current branch's history</td>
		</tr>
	</tbody>
</table>
<h3>Inspect & Compare</h3>
<h4>Examining logs, diffs and object information</h4>
<table>
	<tbody>
		<tr>
			<td>git log</td><td>Show the  commit history for the currently active branch</td>
		</tr>
		<tr>
			<td>git log branchB..branchA</td><td>Show the commits on <em>branchA</em> that are not on <em>branchB</em></td>
		</tr>
		<tr>
			<td>git log --follow [file]</td><td>Show the commits that changed <em>file</em>, even across renames</td>
		</tr>
		<tr>
			<td>git diff branchB...branchA</td><td>Show the diff of what is in <em>branchA</em> that is not in <em>branchB</em></td>
		</tr>
		<tr>
			<td>git show [SHA]</td><td>Show any object in Git in human-readable format</td>
		</tr>
	</tbody>
</table>
<h3>Tracking path changes</h3>
<h4>Versioning file removes and path changes</h4>
<table>
	<tbody>
		<tr>
			<td>git rm [file]</td><td>Deletes <em>file</em> from project and stage the removal for commit</td>
		</tr>
		<tr>
			<td>git mv existing-path new-path</td><td>Change an existing file path and stage the move</td>
		</tr>
		<tr>
			<td>git log --stat -M</td><td>Show all commit logs with indication of any paths that moved</td>
		</tr>
	</tbody>
</table>
<h3>Ignoring Patterns</h3>
<h4>Preventing unintentional staging or committing files</h4>
<p><em>logs/</em></p>
<p><em>*.notes</em></p>
<p><em>pattern*/</em></p>
<p>Save a file with desired patterns as .gitignore with either direct string matches or wildcard globs.</p>
<table>
	<tbody>
		<tr>
			<td>git config --global core.excludesefile [file]</td><td>Systemwide ignore pattern for all local repositories</td>
		</tr>
	</tbody>
</table>
<h3>Share & Update</h3>
<h4>Retrieving updates from another repository and updating local repos</h4>
<table>
	<tbody>
		<tr>
			<td>git remote add [alias] [url]</td><td>Add a git <em>url</em> as an <em>alias</em></td>
		</tr>
		<tr>
			<td>git fetch [alias]</td><td>Fetch down all the branches from that Git remote</td>
		</tr>
		<tr>
			<td>git merge [alias]/[branch]</td><td>Merge a remote branch into your current branch to bring it up to date</td>
		</tr>
		<tr>
			<td>git push [alias] [branch]</td><td>Transmit local branch commits to the remote repository branch</td>
		</tr>
		<tr>
			<td>git pull</td><td>Fetch and merge any commits from the tracking remote branch</td>
		</tr>
	</tbody>
</table>
<h3>Rewrite history</h3>
<h4>Rewriting branches, updating commits and clearing history</h4>
<table>
	<tbody>
		<tr>
			<td>git rebase [branch]</td><td>Apply any commits of current branch ahead of specified one</td>
		</tr>
		<tr>
			<td>git reset --hard [commit]</td><td>Clear staging area, rewrite working tree from specified commit</td>
		</tr>
	</tbody>
</table>
<h3>Temporary commits</h3>
<h4>Temporarily store modified, tracked files in order to change branches</h4>
<table>
	<tbody>
		<tr>
			<td>git stash</td><td>Save modified and staged changes</td>
		</tr>
		<tr>
			<td>git stash list</td><td>List stack-order of stashed file changes</td>
		</tr>
		<tr>
			<td>git stash pop</td><td>Write working from top of stash stack</td>
		</tr>
		<tr>
			<td>git stash drop</td><td>Discard the changes from top of stash stack</td>
		</tr>
	</tbody>
</table>
