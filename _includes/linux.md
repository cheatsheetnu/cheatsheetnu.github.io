<h3>System Info</h3>
<table>
	<tbody>
		<tr>
			<td>date</td><td>Show the current date and time</td>
		</tr>
		<tr>
			<td>cal</td><td>Show this month's calendar</td>
		</tr>
		<tr>
			<td>uptime</td><td>Show current uptime</td>
		</tr>
		<tr>
			<td>w</td><td>Display who is online</td>
		</tr>
		<tr>
			<td>whoami</td><td>Who you are logged in as</td>
		</tr>
		<tr>
			<td>finger user</td><td>Display information about <em>user</em></td>
		</tr>
		<tr>
			<td>uname -a</td><td>Show kernel information</td>
		</tr>
	</tbody>
</table>
<h3>File Commands</h3>
<table>
	<tbody>
		<tr>
			<td>ls</td><td>Directory listing</td>
		</tr>
		<tr>
			<td>ls -l</td><td>List files in current directory using long format</td>
		</tr>
		<tr>
			<td>ls -laC</td><td>List all files in current directory in long format and display in columns</td>
		</tr>
		<tr>
			<td>ls -F</td><td>List files in current directory and indicate the file type</td>
		</tr>
		<tr>
			<td>ls -al</td><td>Formatted listing with hidden files</td>
		</tr>
		<tr>
			<td>tree</td><td>Directory listing in tree format</td>
		</tr>
		<tr>
			<td>cd dir</td><td>Change directory to <em>dir</em></td>
		</tr>
		<tr>
			<td>cat /proc/cpuinfo</td><td>CPU information</td>
		</tr>
		<tr>
			<td>cat /proc/meminfo</td><td>Memory information</td>
		</tr>
		<tr>
			<td>df -h</td><td>Show disk usage</td>
		</tr>
		<tr>
			<td>du</td><td>Show directory space usage</td>
		</tr>
		<tr>
			<td>free</td><td>Show memory and swap usage</td>
		</tr>
	</tbody>
</table>
<h3>Learn the commands</h3>
<table>
	<tbody>
		<tr>
			<td>apropos subject</td><td>List manual pages for <em>subject</em></td>
		</tr>
		<tr>
			<td>man -k keyword</td><td>Display man pages containing <em>keyword</em></td>
		</tr>
		<tr>
			<td>man command</td><td>Show the manual for <em>command</em></td>
		</tr>
		<tr>
			<td>man -t command | ps2pdf -> command.pdf</td><td>Make a pdf of a manual page</td>
		</tr>
		<tr>
			<td>which command</td><td>Show full path name of <em>command</em></td>
		</tr>
		<tr>
			<td>time command</td><td>See how long a <em>command</em> takes</td>
		</tr>
		<tr>
			<td>whereis app</td><td>Show possible lcoations of <em>app</em></td>
		</tr>
		<tr>
			<td>which app</td><td>Show which <em>app</em> will be run by default; it shows the full path</td>
		</tr>
	</tbody>
</table>
<h3>Searching</h3>
<table>
	<tbody>
		<tr>
			<td>grep pattern files</td><td>Search for <em>pattern</em> in <em>files</em></td>
		</tr>
		<tr>
			<td>grep -r pattern dir</td><td>Search recusrively for <em>pattern</em> in <em>dir</em></td>
		</tr>
		<tr>
			<td>command | grep pattern</td><td>Search for <em>pattern</em> in the output of <em>command</em></td>
		</tr>
		<tr>
			<td>locate file</td><td>Find all instances of <em>file</em></td>
		</tr>
		<tr>
			<td>find / -name filename</td><td>Starting with the root directory, look for the file called <em>filename</em></td>
		</tr>
		<tr>
			<td>find / -name "*filename*</td><td>Starting with the root directory, look for the file containing the string <em>filename</em></td>
		</tr>
		<tr>
			<td>locate file</td><td>Find all instances of <em>file</em></td>
		</tr>
		<tr>
			<td>updatedb</td><td>Create or update the database of files on all file systems attached to the Linux root directory</td>
		</tr>
		<tr>
			<td>which filename</td><td>Show the subdirectory containing hte executalbe file called <em>filename</em></td>
		</tr>
		<tr>
			<td>grep TextStringToFind /dir</td><td>Starting with the directory called <em>dir</em>, look for and list all files containing <em>TextStringToFind</em></td>
		</tr>
	</tbody>
</table>
<h3>File Permissions</h3>
<table>
	<tbody>
		<tr>
			<td>chmod octal file</td><td>Change the permissions of <em>file</em> to <em>octal</em> which can be found separately for user, group and world by adding: 4 - read (r), 2 - write (w), 1 - execute (x)</td>
		</tr>
		<tr>
			<td>chmod 777</td><td>read, write, execute for all</td>
		</tr>
		<tr>
			<td>chmod 755</td><td>rwx for owner, rx for group and world. For more options see <em>man chmod.dir</em></td>
		</tr>
		<tr>
			<td>cd</td><td>Change to home</td>
		</tr>
		<tr>
			<td>mkdir dir</td><td>Create a directory <em>dir</em></td>
		</tr>
		<tr>
			<td>pwd</td><td>Show current directory</td>
		</tr>
		<tr>
			<td>rm name</td><td>Remove a file or directory called <em>name</em></td>
		</tr>
		<tr>
			<td>rm -r dir</td><td>Delete directory <em>dir</em></td>
		</tr>
		<tr>
			<td>rm -f file</td><td>Force remove <em>file</em></td>
		</tr>
		<tr>
			<td>rm -rf dir</td><td>Force remove an entire directory <em>dir</em> and all it's included files and subdirectories (use with extreme caution)</td>
		</tr>
		<tr>
			<td>cp file1 file2</td><td>Copy <em>file1</em> to <em>file2</em></td>
		</tr>
		<tr>
			<td>cp -r dir1 dir2</td><td>Copy <em>dir1</em> to <em>dir2</em>; create <em>dir2</em> if it doesn't exist</td>
		</tr>
		<tr>
			<td>cp file /home/dirname</td><td>Copy <em>file</em> to the <em>/home/dirname</em> directory</td>
		</tr>
		<tr>
			<td>mv file /home/dirname</td><td>Move the <em>file</em> to the <em>/home/dirname</em> directory</td>
		</tr>
		<tr>
			<td>mv file1 file2</td><td>Rename or move <em>file1</em> to <em>file2</em>; if <em>file2</em></td>
		</tr>
		<tr>
			<td>ln -s file link</td><td>Create symbolic link <em>link</em> to <em>file</em></td>
		</tr>
		<tr>
			<td>touch file</td><td>Create or update <em>file</em></td>
		</tr>
		<tr>
			<td>cat > file</td><td>Places standard input into <em>file</em></td>
		</tr>
		<tr>
			<td>cat file</td><td>Display the file called <em>file</em></td>
		</tr>
		<tr>
			<td>more file</td><td>Display the file called <em>file</em> one page at a time, proceed to next page using the spacebar</td>
		</tr>
		<tr>
			<td>head file</td><td>Output the first 10 lines of the file called <em>file</em></td>
		</tr>
		<tr>
			<td>head - 20 file</td><td>Output the first 20 lines of the file called <em>file</em></td>
		</tr>
		<tr>
			<td>tail file</td><td>Output the last 10 lines of the file called <em>file</em></td>
		</tr>
		<tr>
			<td>tail -20 file</td><td>Output the last 20 lines of the file called <em>file</em></td>
		</tr>
		<tr>
			<td>tail -f file</td><td>Output the contents of <em>file</em> as it grows, starting with the last 10 lines</td>
		</tr>
	</tbody>
</table>
<h3>Compression</h3>
<table>
	<tbody>
		<tr>
			<td>tar cf file.tar files</td><td>Create a tar named <em>file.tar</em> containing <em>files</em></td>
		</tr>
		<tr>
			<td>tar xf file.tar</td><td>Extract the files from <em>file.tar</em></td>
		</tr>
		<tr>
			<td>tar czf file.tar.gz files</td><td>Create a tar with Gzip compression</td>
		</tr>
		<tr>
			<td>tar xzf file.tar.gz</td><td>Extract a tar using Gzip</td>
		</tr>
		<tr>
			<td>tar cjf file.tar.bz2</td><td>Create a tar with Bzip2 compression</td>
		</tr>
		<tr>
			<td>tar xjf file.tar.bz2</td><td>Extract a tar using Bzip2</td>
		</tr>
		<tr>
			<td>gzip file</td><td>Compresses <em>file</em> and renames it to <em>file.gz</em></td>
		</tr>
		<tr>
			<td>gzip -d file.gz</td><td>Decompresses <em>file.gz</em> back to <em>file</em></td>
		</tr>
	</tbody>
</table>
<h3>Network</h3>
<table>
	<tbody>
		<tr>
			<td>ifconfig</td><td>List IP addresses for all devices on the local machine</td>
		</tr>
		<tr>
			<td>iwconfig</td><td>Used to set the parameters of the network interface which are specific to the wireless operation (for exmple: the frequency)</td>
		</tr>
		<tr>
			<td>iwlist</td><td>Used to display some additional information from a wireless network interface that is not displayed by <em>iwconfig</em></td>
		</tr>
		<tr>
			<td>ping host</td><td>Ping <em>host</em> and output results</td>
		</tr>
		<tr>
			<td>whois domain</td><td>Get whois information for <em>domain</em></td>
		</tr>
		<tr>
			<td>dig domain</td><td>Get DNS information for <em>domain</em></td>
		</tr>
		<tr>
			<td>dig -x host</td><td>Reverse lookup <em>host</em></td>
		</tr>
		<tr>
			<td>wget file</td><td>Download <em>file</em></td>
		</tr>
		<tr>
			<td>wget -c file</td><td>Continue a stopped download</td>
		</tr>
	</tbody>
</table>
<h3>SSH</h3>
<table>
	<tbody>
		<tr>
			<td>ssh user@host</td><td>Connect to <em>host</em> as <em>user</em></td>
		</tr>
		<tr>
			<td>ssh -p port user@host</td><td>Connect to <em>host</em> on port <em>port</em> as <em>user</em></td>
		</tr>
		<tr>
			<td>ssh-copy-id user@host</td><td>Add your key to <em>host</em> for <em>user</em> to enable a keyed or passwordless login</td>
		</tr>
	</tbody>
</table>
<h3>User Administration</h3>
<table>
	<tbody>
		<tr>
			<td>adduser accountname</td><td>Create a new user called <em>accountname</em></td>
		</tr>
		<tr>
			<td>passwd accountname</td><td>Give <em>accountname</em> a new password</td>
		</tr>
		<tr>
			<td>su</td><td>Login as superuser from current login</td>
		</tr>
		<tr>
			<td>exit</td><td>Stop being superuser and revert to normal user</td>
		</tr>
	</tbody>
</table>
<h3>Process Management</h3>
<table>
	<tbody>
		<tr>
			<td>ps</td><td>Display your currently active processes</td>
		</tr>
		<tr>
			<td>top</td><td>Display all running processes</td>
		</tr>
		<tr>
			<td>htop</td><td>Display all running processes</td>
		</tr>
		<tr>
			<td>kill pid</td><td>Kill process id <em>pid</em></td>
		</tr>
		<tr>
			<td>killall proc</td><td>Kill all processes named <em>proc</em> (use with extreme caution)</td>
		</tr>
		<tr>
			<td>bg</td><td>Lists stopped or background jobs; resume a stopped job in the background</td>
		</tr>
		<tr>
			<td>fg</td><td>Brings the most recent job to foreground</td>
		</tr>
		<tr>
			<td>fg n</td><td>Bring job <em>n</em> to the foreground</td>
		</tr>
	</tbody>
</table>
<h3>Installation from package manager</h3>
<table>
	<tbody>
		<tr>
			<td>apt-get install apache2</td><td>Install Apache2 (Debian / Ubuntu /Linux Mint)</td>
		</tr>
		<tr>
			<td>apt-get install -y apache2</td><td>Install Apache2 without confirm (Debian / Ubuntu /Linux Mint)</td>
		</tr>
		<tr>
			<td>apt-get install -y apache2 && apt-get install -y php-fpm</td><td>Install Apache2 and PHP-FPM without confirm</td>
		</tr>
	</tbody>
</table>
<h3>Installation from source</h3>
<table>
	<tbody>
		<tr>
			<td>./configure</td><td></td>
		</tr>
		<tr>
			<td>make</td><td></td>
		</tr>
		<tr>
			<td>make install</td><td></td>
		</tr>
		<tr>
			<td>dpkg -i pkg.deb</td><td>Install a DEB package (Debian / Ubuntu / Linux Mint)</td>
		</tr>
		<tr>
			<td>rpm - Uvh pkg.rpm</td><td>Install an RPM package (Red Hat / Fedora)</td>
		</tr>
	</tbody>
</table>
<h3>Stopping & Starting</h3>
<table>
	<tbody>
		<tr>
			<td>shutdown -h now</td><td>Shutdown the system now and do not reboot</td>
		</tr>
		<tr>
			<td>halt</td><td>Stop all processes - same as above</td>
		</tr>
		<tr>
			<td>shutdown -r 5</td><td>Shutdown the system in 5 minutes and reboot</td>
		</tr>
		<tr>
			<td>shutdown -r now</td><td>Shutdown the system now and reboot</td>
		</tr>
		<tr>
			<td>reboot</td><td>Stop all processes and then reboot - same as above</td>
		</tr>
		<tr>
			<td>service apache2 start|stop|restart</td><td>Start the Apache2 system</td>
		</tr>
		<tr>
			<td>service varnish start|stop|restart</td><td>Star the Varnish system</td>
		</tr>
	</tbody>
</table>
