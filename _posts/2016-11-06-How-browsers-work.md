
A
web browser is a program that retrieves documents from remote servers
and displays them on screen, either within the browser window itself
or by passing the document to an external helper applications. It
allows particular resources to be requested explicitly by URI, or
implicitly by following embedded hyperlinks.

-To
look at how the web browser works, we need to look at the components
and structure of the web browser itself.

-The
most basic component in web browsers are the web pages.

-There
are probably as many web pages on the web today as there are neurons
in your head, or as there are stars in the milky way.

-Web
pages are written in;

- HTML(Hyper
	Text Mark-up Language)-This code tells web browsers how to structure
	and present contents on a web page.  
- CSS(Cascading
	Style Sheets)- allows authors to add layout and style information to
	web pages, without complicating the original structural mark up. 
- Java
	Script- is a host environment for performing client-side
	computations E.g altering page and image loading behaver,
	interpreting mouse actions etc. 

-The
web browser is perhaps the most widely used software application in
history. 

-It
has evolved significantly over the past fifteen years; today, web
browsers run on diverse types of hardware, from cell phones and
tablet PCs to desktop computers.

_-Old browsers can negatively impact our
mordern lives, and that is something most people fail to realise.
Particularly on our online safety._

_-Updating to a mordern web browser is
important for three main reasons;_

_1. Old browsers are vulnerable to attacks,
because they typically arent updated with the latest security fixes
and fixtures. Browsing with such could lead to stolen passwords,
malicious s/w snuck secretely into your machine, phishing or even
worse._

_2.The World Wide Web evolves fast, and with
such, most of the features available on today's websites and web
applications wont work with old browsers_

_3.Old browsers slow down innovation on the
web. If lots of internet users choose to cling to old browsers, web
developers are then forced to design websites that work with both old
and new techz_

-Applications
are also called programs or software. In the online world of web
browsers and smart phones, apps are usually nimbler programs focused
on a single task. Web apps, run these tasks inside the web browser
and often provide a rich and interactive experience.

-Merits
of using web apps are;

		1.It
works on ever device with a web browsers

		2.I
can access my data from anywhere

		3.
I'll always get the latest version of any application

		4.
It is ideally a safer approach to browsing.

-
Using the source code and available architecture of two mature web
browsers implementation,ie Mozilla and Konqueror a reference
architecture was derived for the web browser.

_The Reference architecture later derived had 8
subsytems;_

_1.**The User Interface Subsystem **-Provides
features such as toolbars, visual page-load progress, smart download
handling and printing. It may be intergrated with the desktop
environment to provide browser session management or communication
with other applications._

_2.**The
Browser Engine Subsytem – **It
provides high-level interface to the Rendering Engine. Ie it loads a
given URI and supports primitive browsing actions eg forwarding, back
and reload_

_- It also provides hooks for viewing various
aspects of the browsing session such as page load progress and
JavaScript alerts._

_3.**The
rendering Engine Subsytem – **Provides
a visual representation for a given URI and is capable of displaying
HTML and extensible Mark-Up language(XML) docz, optionally styled
with CSS, as well as embeded content such as images.It
calculates the exact _

_page layout and may use “reflow”
algorithms to incrementally adjust the position of elements on the
page.Also includes the HTML parser_

_4.**The
Networking Subsystem –**
Implements file transfer
protocols such as HTTP and FTP. It may implement a cache of recently
retrieved resources, also translates different character sets and
resolves MIME media types for files._

_5.**The
JavaScript Interpreter – **Evaluates
JS code, which may be embedded in web pages. Certain JS functionality
such as opening of pop-up windows, may be disabled by the browser
engine or Rendering Engine for security purposes._

_6.**The
XML Parser Subsytem –** Parses
XML documents into a Document Object Model(DOM) tree. One of th emost
re-usable sub systems in the architecture, infact almost all browsers
leverage an existing XML Parser rather than creating their own._

_7.**The
display Backend Subsytem –**
Provides drawing and
windowing primitives, a set
of user interface widgets and a set of fonts. Could be tied closely
with the OS_

_8.**The
Data Persistence Subsystem –**
Stores various data
associated with the browsing session on disk. E.g bookmarks, toolbar
settings, cookies, security certificates or cache._
