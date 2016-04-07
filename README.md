# Frederiksberg-beamer-theme
Copy from the original website that went offline in late 2015

<div class="text" id="content">
This is the home page for the <i>Frederiksberg</i> beamer theme
(for typesetting presentation slides in LaTeX).

<h2>Installation</h2>

Get either the <tt>.tgz</tt> (Linux/Mac) or <tt>.zip</tt> (Windows) file(s)
from the <a href="#">download page</a>.

<ul>
<li><b>Windows</b>, using MiKTeX (2.7 or 2.8):
<ol>
<li>Find your local TeX installation directory, probably
<tt>C:\localtexmf</tt><br/>
If this does not exist: Create it.</li>
<li>Make certain that the directory you found/created is one of MiKTeX's
roots:<br/>
Under your programs menu, open <i>MiKTeX 2.X, Maintenance (Admin), Settings
(Admin)</i> (or without the (Admin), if that is not in your menus).<br/>
Click the "Roots" tab. If the directory is not listed in the box, add it.</li>
<li>If you are upgrading from a version 1.x of <i>Frederiksberg</i>,
find and delete the subdirectories <tt>dvips\KULIFE</tt> and
<tt>tex\latex\beamer\KULIFE</tt> and all their content.</li>
<li>If you are upgrading from a version 2.x of <i>Frederiksberg</i>,
find and delete the subdirectories <tt>dvips\Frederiksberg</tt>,
<tt>tex\latex\beamer\Frederiksberg</tt> and <tt>texmf</tt> and all their
content. (That last subdirectory would be e.g. <tt>C:\localtexmf\texmf</tt> and
is only present if you have installed <i>Frederiksberg</i> from a buggy zip
file that was unfortunately downloadable from here for quite a while.)</li>
<li>Unzip the file <tt>Frederiksberg-2-2.zip</tt> file into your
local TeX installation directory.</li>
<li>Optionally install a <a href="units/">unit package</a> for
your KU unit or department (if availale) by unzipping the package <tt>.zip</tt>
file into your local TeX installation directory.</li>
<li>Update the MiKTeX file name database:<br/>
Under your programs menu, open <i>MiKTeX 2.X, Maintenance (Admin), Settings
(Admin)</i> (or without the (Admin), if that is not in your menus).<br/>
Under the "General" tab, click "Refresh FNDB".</li>
</ol>
</li>
<li><b>Linux</b> (works with my SuSE and Jakob's Ubuntu, both with TeX Live):
<pre class="code">
sudo mkdir /usr/local/share/texmf
cd /usr/local/share/texmf
sudo rm -rf dvips/KULIFE tex/latex/beamer/KULIFE
sudo rm -rf dvips/Frederiksberg tex/latex/beamer/Frederiksberg texmf
sudo tar xzf /path-to-the-file/Frederiksberg-2-2.tgz
# Install a unit package, if available:
# sudo tar xzf /path-to-the-file/myunit.tgz
sudo texhash
</pre>
Note that this assumes your local TeX files are supposed to be in the
directory <tt>/usr/local/share/texmf</tt> - and that the first line above
(beginning <tt>sudo mkdir</tt>) is only required if this directory does
not already exist.
If the commands above work for you, this is the proper location.
Otherwise you may want to check the supposed location by looking
in the file <tt>texmf.cnf</tt> which will probably either be at
<tt>/etc/texmf/web2c/texmf.cnf</tt> or <tt>/etc/texmf/texmf.cnf</tt>.
<br/>
Note that the <tt>sudo rm</tt> lines are only needed if you are upgrading
from a previous version of <i>Frederiksberg</i>.
<br/>
Note also that the commented <tt>sudo tar</tt> command should only be run
(uncommented) if you have a <a href="units/">unit package</a> to install.
</li>
<li><b>Mac OS X</b> with gwTeX based on TeX Live:<br/>
You can install either for all users or for one user.
You must open a terminal and run the commands below (yes, I know, this is very
un-Mac'ish but I work with the Mac mainly through its Unix command line
interface).
<ul><li>Install for all users:
<pre class="code">
cd /usr/local/gwTeX/texmf.local
sudo rm -rf dvips/KULIFE tex/latex/beamer/KULIFE
sudo rm -rf dvips/Frederiksberg tex/latex/beamer/Frederiksberg texmf
sudo tar xzf /path-to-the-file/Frederiksberg-2-2.tgz
# Install a unit package, if available:
# sudo tar xzf /path-to-the-file/myunit.tgz
sudo texhash
</pre>
The <tt>sudo rm</tt> lines are only needed if you are upgrading from a previous
version of <i>Frederiksberg</i>.
The commented <tt>sudo tar</tt> command should only be run
(uncommented) if you have a <a href="units/">unit package</a> to install.
</li>
<li>Install for yourself only (current user):
<pre class="code">
cd ~/Library
mkdir texmf
cd texmf
rm -rf dvips/KULIFE tex/latex/beamer/KULIFE
rm -rf dvips/Frederiksberg tex/latex/beamer/Frederiksberg texmf
tar xzf /path-to-the-file/Frederiksberg-2-2.tgz
# Install a unit package, if available:
# tar xzf /path-to-the-file/myunit.tgz
</pre>
The <tt>mkdir</tt> line above is only needed if your <tt>Library</tt>
directory does not already contain the <tt>texmf</tt> directory.
The <tt>rm</tt> lines are only needed if you are upgrading from a previous
version of <i>Frederiksberg</i>.
The commented <tt>tar</tt> command should only be run
(uncommented) if you have a <a href="units/">unit package</a> to install.
</li>
</ul>
</li>

<li><b>Mac OS X</b> with
<a href="https://web.archive.org/web/20150605233943/http://www.tug.org/mactex/">MacTex 2010</a> (also based on TeX Live):<br/>
A user has reported that the recipy given for gwTeX above should work, with
a different installation path. Only a path for all users has been reported:
<ul><li>Install for all users:
<pre class="code">
cd /usr/local/texlive/2010/texmf/
sudo rm -rf dvips/KULIFE tex/latex/beamer/KULIFE
sudo rm -rf dvips/Frederiksberg tex/latex/beamer/Frederiksberg texmf
sudo tar xzf /path-to-the-file/Frederiksberg-2-2.tgz
# Install a unit package, if available:
# sudo tar xzf /path-to-the-file/myunit.tgz
sudo texhash
</pre>
The <tt>sudo rm</tt> lines are only needed if you are upgrading from a previous
version of <i>Frederiksberg</i>.
The commented <tt>sudo tar</tt> command should only be run
(uncommented) if you have a <a href="units/">unit package</a> to install.
</li>
</ul>
</li>
</ul>
</div>
<div id="footer"><div class="text">
<a href="https://web.archive.org/web/20150605233943/http://www.matdat.life.ku.dk/~henrikp" title="Henrik's home page">Henrik Laurberg Pedersen</a>&nbsp;<a href="mailto:henrikp@life.ku.dk" title="Send mail to Henrik">&lt;henrikp@life.ku.dk&gt;</a> | Last change: 2011-05-13</div></div>
