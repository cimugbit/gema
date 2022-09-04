# General Purpose Text Processor

This is Gema, David N Gray's wonderful pattern matching engine. I have started
using it in 2009, and it did wonders for me. When I switched from AIX to Linux
some years later, I got segmentation faults in certain scripts. Using Valgrind
I was able to find a double-free error as the cause which I could fix with a
small code change.

The original Gema project homepage is not available any more. Gema
code is now at https://sourceforge.net/projects/gema/files/gema/, including a
Git repository with some recent development
(https://git.code.sf.net/p/gema/code.git). However, when I built the master
branch on 2022-09-04, the tests failed.

Karolin Varner seems to have cloned the old CVS with the full commmit histoy
before it disappeared (https://github.com/koraa/gema), however this is
still the original code from 2004 with the double free error I discovered.

So I decided to conserve my Gema version into a public Git repository to share
it and keep Gema alive. I haven't checked the code with Valgrind again after
reading Karolin's statement, but after I fixed the double free error years ago,
I haven't experienced any crashes. I would, however, support Karolin's vote to
not feed untrusted input to it. I also suspect the problems I occasionally had
in my scripts are not all due to my own lack of understanding. But anyway -
Gema is a great tool!

I added to this repository the Gema HTML documentation I downloaded in
2009 and David A. Mundie's inspiring article about Gema that also disappeared
from where I downloaded it. Also, as I do with all reference documentation, I
supplied the Gema Reference with a TOC outline on the left side for convenient
reading and navigation.

In the contrib directory, I also added the script template from which I derive
every new Gema script and which I refined over time, as well as the NEdit syntax
highlighting patterns I created when I started using Gema. I wouldn't have had
so much fun writing Gema scripts without them since Gema scripts are hard enough
to read even with syntax highlighting.
