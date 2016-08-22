---
layout: post
title: VI Commands
---

<h2><a name="vi">VI Commands</a></h2>
<h3>Basics</h3>
<table>
<tr>
<td>:e filename</td><td>Open <em>filename</em> for edition</td>
</tr>
<tr>
<td>:w</td><td>Save file</td></tr><tr><td
>:q</td><td>Exit Vim</td></tr><tr><td
>:w!</td><td>Write file and quit</td></tr></table>
<h2>Search</h2>
<table>
<tr><td
>/word</td><td>Search <em>word</em> from top to bottom</td></tr><tr><td
>?word</td><td>Search <em>word</em> from bottom to top</td></tr><tr><td
>/jo[ha]n</td><td>Search <em>john</em> or <em>joan</em></td></tr><tr><td
>/\&lt; the</td><td>Search the, theatre or <em>then</em></td></tr><tr><td
>/the\&gt;</td><td>Search <em>the</em> or <em>breathe</em></td></tr><tr><td
>/\&lt; the\&gt;</td><td>Search <em>the</em></td></tr><tr><td
>/\&lt; </em>¦.\&gt;</td><td>Search all words of 4 letters</td></tr><tr><td
>/\/</td><td>Search <em>fred</em> but not <em>alfred</em> or <em>frederick</em></td></tr><tr><td
>/fred\|joe</td><td>Search <em>fred</em> or <em>joe</em></td></tr><tr><td
>/\&lt;\d\d\d\d\&gt;</td><td>Search exactly 4 digits</td></tr><tr><td
>/^\n\{3}</td><td>Find 3 empty lines</td></tr><tr><td
>:bufdo /searchstr/</td><td>Search in all open files</td></tr</table>
<h2>Replace</h2>
<table><tr><td>:%s/old/new/g</td><td>Replace all occurences of <em>old</em> by <em>new</em> in file</td></tr><tr><td
>:%s/old/new/gw</td><td>Replace all occurences with confirmation</td></tr><tr><td
>:2,35s/old/new/g</td><td>Replace all occurences between lines 2 and 35</td></tr><tr><td
>:5,$s/old/new/g</td><td>Replace all occurences from line 5 to EOF</td></tr><tr><td
>:%s/^/hello/g</td><td>Replace the begining of each line by <em>hello</em></td></tr><tr><td
>:%s/$/Harry/g</td><td>Replace the end of each line by <em>Harry</em></td></tr><tr><td
>:%s/onward/forward/gi</td><td>Replace <em>onward</em> by <em>forward</em>, case unsensitive</td></tr><tr><td
>:%s/ *$//g</td><td>Delete all white spaces</td></tr><tr><td
>:g/string/d</td><td>Delete all lines containing <em>string</em></td></tr><tr><td
>:v/string/d</td><td>Delete all lines containing which didn&#8217;t contain <em>string</em></td></tr><tr><td
>:s/Bill/Steve/</td><td>Replace the first occurence of <em>Bill</em> by <em>Steve</em> in current line</td></tr><tr><td
>:s/Bill/Steve/g</td><td>Replace <em>Bill</em> by <em>Steve</em> in current line</td></tr><tr><td
>:%s/Bill/Steve/g</td><td>Replace <em>Bill</em> by <em>Steve</em> in all the file</td></tr><tr><td
>:%s/\r//g</td><td>Delete DOS carriage returns (^M)</td></tr><tr><td
>:%s/\r/\r/g</td><td>Transform DOS carriage returns in returns</td></tr><tr><td
>:%s#&lt;[^&gt;]\+&gt;##g</td><td>Delete HTML tags but keeps text</td></tr><tr><td
>:%s/^\(.*\)\n\1$/\1/</td><td>Delete lines which appears twice</td></tr><tr><td
>Ctrl+a</td><td>Increment number under the cursor</td></tr><tr><td
>Ctrl+x</td><td>Decrement number under cursor</td></tr><tr><td
>ggVGg?</td><td>Change text to Rot13</td></tr></table><h2 id="casse">Case</h2>
<table><tr><td
>Vu</td><td>Lowercase line</td></tr><tr><td
>VU</td><td>Uppercase line</td></tr><tr><td
>g~~</td><td>Invert case</td></tr><tr><td
>vEU</td><td>Switch word to uppercase</td></tr><tr><td
>vE~</td><td>Modify word case</td></tr><tr><td
>ggguG</td><td>Set all text to lowercase</td></tr><tr><td
>:set ignorecase</td><td>Ignore case in searches</td></tr><tr><td
>:set smartcase</td><td>Ignore case in searches excepted if an uppercase letter is used</td></tr><tr><td
>:%s/\&lt;./\u&amp;/g</td><td>Sets first letter of each word to uppercase</td></tr><tr><td
>:%s/\&lt;./\l&amp;/g</td><td>Sets first letter of each word to lowercase</td></tr><tr><td
>:%s/.*/\u&amp;</td><td>Sets first letter of each line to uppercase</td></tr><tr><td
>:%s/.*/\l&amp;</td><td>Sets first letter of each line to lowercase</td></tr></table>
<h2>Read/Write files</h2>
<table><tr><td>:1,10 w outfile</td><td>Saves lines 1 to 10 in <em>outfile</em></td></tr><tr><td
>:1,10 w &gt;&gt; outfile</td><td>Appends lines 1 to 10 to <em>outfile</em></td></tr><tr><td
>:r infile</td><td>Insert the content of <em>infile</em></td></tr><tr><td
>:23r infile</td><td>Insert the content of <em>infile</em> under line 23</td></tr></table>
<h2 id="explorateur">File explorer</h2>
<table><tr><td
>:e .</td><td>Open integrated file explorer</td></tr><tr><td
>:Sex</td><td>Split window and open integrated file explorer</td></tr><tr><td
>:browse e</td><td>Graphical file explorer</td></tr><tr><td
>:ls</td><td>List buffers</td></tr><tr><td
>:cd ..</td><td>Move to parent directory</td></tr><tr><td
>:args</td><td>List files</td></tr><tr><td
>:args *.php</td><td>Open file list</td></tr><tr><td
>:grep expression *.php</td><td>Returns a list of .php files contening <em>expression</em></td></tr><tr><td
>gf</td><td>Open file name under cursor</td></tr></table>
<h2 id="unix">Interact with Unix</h2>
<table><tr><td>:!pwd</td><td>Execute the <em>pwd</em> unix command, then returns to Vi</td></tr>
<tr><td>!!pwd</td><td>Execute the <em>pwd</em> unix command and insert output in file</td></tr><tr><td
>:sh</td><td>Temporary returns to Unix</td></tr><tr><td
>$exit</td><td>Retourns to Vi</td></tr></table>
<h2 id="alignement">Alignment</h2>
<table><tr><td>:%!fmt</td><td>Align all lines</td></tr><tr><td
>!}fmt</td><td>Align all lines at the current position</td></tr><tr><td
>5!!fmt</td><td>Align the next 5 lines</td></tr></table>
<h2 id="onglets">Tabs</h2>
<table><tr><td>:tabnew</td><td>Creates a new tab</td></tr><tr><td
>gt</td><td>Show next tab</td></tr><tr><td
>:tabfirst</td><td>Show first tab</td></tr><tr><td
>:tablast</td><td>Show last tab</td></tr><tr><td
>:tabm n(position)</td><td>Rearrange tabs</td></tr><tr><td
>:tabdo %s/foo/bar/g</td><td>Execute a command in all tabs</td></tr><tr><td
>:tab ball</td><td>Puts all open files in tabs</td></tr></table>
<h2 id="partage">Window spliting</h2>
<table><tr><td>:e filename</td><td>Edit <em>filename</em> in current window</td></tr><tr><td
>:split filename</td><td>Split the window and open <em>filename</em></td></tr><tr><td
>ctrl-w up arrow</td><td>Puts cursor in top window</td></tr><tr><td
>ctrl-w ctrl-w</td><td>Puts cursor in next window</td></tr><tr><td
>ctrl-w_</td><td>Maximise current window</td></tr><tr><td
>ctrl-w=</td><td>Gives the same size to all windows</td></tr><tr><td
>10 ctrl-w+</td><td>Add 10 lines to current window</td></tr><tr><td
>:vsplit file</td><td>Split window vertically</td></tr><tr><td
>:sview file</td><td>Same as <strong>:split</strong> in readonly mode</td></tr><tr><td
>:hide</td><td>Close current window</td></tr><tr><td
>:&#173;nly</td><td>Close all windows, excepted current</td></tr><tr><td
>:b 2</td><td>Open #2 in this window</td></tr></table>
<h2 id="completion">Auto-completion</h2>
<table><tr><td
>Ctrl+n Ctrl+p (in insert mode)</td><td>Complete word</td></tr><tr><td
>Ctrl+x Ctrl+l</td><td>Complete line</td></tr><tr><td
>:set dictionary=dict</td><td>Define <em>dict</em> as a dictionnary</td></tr><tr><td
>Ctrl+x Ctrl+k</td><td>Complete with dictionnary</td></tr></table>
<h2 id="marqueurs">Marks</h2>
<table><tr><td>mk</td><td>Marks current position as <em>k</em></td></tr><tr><td
></em>˜k</td><td>Moves cursor to mark <em>k</em></td></tr><tr><td
>d</em>™k</td><td>Delete all until mark <em>k</em></td></tr></table>
<h2 id="abbr">Abbreviations</h2>
<table><tr><td>:ab mail mail@provider.org</td><td>Define <em>mail</em> as abbreviation of <em>mail@provider.org</em></td></tr></table>
<h2 id="indentation">Text indent</h2>
<table><tr><td>:set autoindent</td><td>Turn on auto-indent</td></tr><tr><td
>:set smartindent</td><td>Turn on intelligent auto-indent</td></tr><tr><td
>:set shiftwidth=4</td><td>Defines 4 spaces as indent size</td></tr><tr><td
>ctrl-t, ctrl-d</td><td>Indent/un-indent in insert mode</td></tr><tr><td
>&gt;&gt;</td><td>Indent</td></tr><tr><td>&lt;&lt;</td><td>Un-indent</td></tr>
</table>
<h2 id="coloration">Syntax highlighting</h2>
<table>
<tr><td>:syntax on</td><td>Turn on syntax highlighting</td></tr>
<tr><td>:syntax off</td><td>Turn off syntax highlighting</td></tr><tr><td>:set syntax=perl</td><td>Force syntax highlighting</td></tr>
</table>
