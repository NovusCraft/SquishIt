SquishIt!
=
SquishIt lets you easily compress and combine JavaScript and CSS. It also includes the ability to use dotless to process your CSS.

Installation
-
**Install via NuGet**<br />
The quickest way to get install SquishIt is via [NuGet](http://docs.nuget.org/docs/start-here/overview).

Open [Package Manager console](http://docs.nuget.org/docs/start-here/using-the-package-manager-console) and enter:

	Install-Package SquishIt

**Download from GitHub**<br />

Visit [SquishIt download page](https://github.com/jetheredge/SquishIt/downloads) to donwload the latest release.

**Compile from source**<br />

SquishIt source code is [hosted on GitHub](https://github.com/jetheredge/SquishIt).

You can pull the latest source using Git or [download a zip of the master branch](https://github.com/jetheredge/SquishIt/zipball/master).

Basic usage
-
**CSS bundling and minification**

	@Html.Raw(SquishIt.Framework.Bundle.Css()
								.Add("~/css/file1.css")
								.Add("~/css/file2.css")
								.Render("~/css/combined_#.css"))

*Explanation*
1. All CSS bundling is handled via `SquishIt.Framework.Bundle.Css()` API.
2. Call `.Add()` method to specify which files to bundle.
3. Call `Render()` method at the end to specify filepath of the generated file

This will combine files in the order they were specified and minify them using Microsoft Minifier.

Advanced usage
-

Contribute
- 
**Report a bug**<br />
If you discover something that doesn't work - please let us know. You could:

* [post a bug report on GitHub](https://github.com/jetheredge/SquishIt/issues/new)
* write a failing test that demonstrates this bug and send a pull request (that would be awesome)
* fix the bug, write some test that prove your bug fix and send a pull request (even more awesome)

**Suggest a feature**<br />
If you have an idea for a new feature:

* [tell us about it](https://github.com/jetheredge/SquishIt/issues/new)
* write a test demonstrating how this feature should work and send a pull request (that would be awesome)
* implemented this feauture + tests and send a pull request (even more awesome)

**Help others**<br />
Have a look at [unanswered SquishIt questions on StackOverflow](http://stackoverflow.com/questions/tagged/squishit?sort=unanswered&pagesize=30) and see if you can answer any of them.<br />
You will help create a library of solutions and lower barrier to entry for new SquishIt users.

**Help keep this document up-to-date**<br />
Documentation has a nasty habit of becoming out of date with reality.<br />
If you can think of a better usage example or spot an error, let us know.<br />
Better yet, update this file and send a pull request.

**Spread the word**<br />
Show SquishIt to your colleagues. Blog it. Tweet it. Spread the word!

Projects using SquishIt
-
Be the first to list your project here... 

Project history
-
Topics:

* Creator (blog?)
* Origin of idea (also when?)
* Original name and new name (Bundler to SquishIt)
* First public release
* Project lead 
* Contributors
* Release schedule

License (MIT)
-
Copyright © 2011-2012, Justin Etheredge - http://www.codethinked.com

Permission is hereby granted, free of charge, to any person obtaining a copy of 
this software and associated documentation files (the "Software"), to deal in the 
Software without restriction, including without limitation the rights to use, copy, 
modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
and to permit persons to whom the Software is furnished to do so, subject to the 
following conditions:

The above copyright notice and this permission notice shall be included in all 
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A 
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT 
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF 
CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE 
OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.