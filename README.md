#Wakanda Modules#
===============

Server-Side Modules for Wakanda Server / WakandaDB

##About##

This repositories is meant to host Wakanda modules provided by the community.
Feel free to send a pull request adding your package as a sub-modules of this repository.

The Wakanda Team provides no guaranty and no support to any submitted package, use them at your own risks…

As in some other marketplaces, the Wakanda Team may highlight a selection of packages for their quality or the features they provide.

##Pre-Requesites##

For the Pull request to be accepted, the repository added as sub-module must contain:

* a <code>README.md</code> file, which should include your copyright and potentially your license text if ,ot too long
* a valid <code>package.json</code> file
* At least one Server-Side JavaScript module called "index.js" or which name is mentionned in the <var>"main"</var> property of the package.json file.

Optional

* a <code>LICENSE</code> file if the license text can not be included in the README file
* unit test files (recommended) to detect limitations, bugs, regressions...

###Package format###

The expected format of the package.json file is directly related to the existing [CommonJS package format](http://wiki.commonjs.org/wiki/Packages/1.0) and [npm package format](https://npmjs.org/doc/json.html).

####a <var>name</var> property####
The name of the package. This must be a unique, lowercase alpha-numeric name without spaces. It may include "." or "_" or "-" characters. It is otherwise opaque.

ex:

```
	"name": "wakanda-supermodule"
```


####a <var>version</var> property####
The most important things in your package.json are the name and version fields. On node.js, those are actually required, and your package won't install without them. The name and version together form an identifier that is assumed to be completely unique. Changes to the package should come along with changes to the version.

A version string conforming to the [Semantic Versioning](http://semver.org/) requirements.

Consider the following version updates: 

* 0.1.0 -> 0.1.1 should be non-breaking. 
* 0.1.1 -> 0.2.0 could be breaking

ex:

```
	"version": "0.1.0"
```

Versions can start with "v".

Creating tags in git like <code>git tag "v1.2.3"</code> for each version is a good practice.

Regarding git again, the Semantic Version rule 3 says 

	3. Once a versioned package has been released, the contents of that version MUST NOT be modified. Any modifications MUST be released as a new version."

So, as also that some may go to check for the last version of your git repository, it is recommended not directly working on a master branch but create a feature  or dev branch and work on it insread.

####a <var>description</var> property####
A brief description of the package. By convention, the first sentence (up to the first ". ") should be usable as a package title in listings.

ex:

```
	"description": "Convert CSV files in JSON."
```

####an <var>author</var> property####
It can be a string or an object describing the Author. 

If it is string, consider the format <code>Full Name < email > (url)</code>

```
	"author": "John Doe <john@doe.com>"
```
As an object, there should be at least one of the fields name, email, or url

```
	"author": {
		"name": "John Doe",
		"email": "john@doe.com",
		"url": "http://john.doe.com"
	}
```
Consider to mention a way to contact you, either email or url. The url might be your personal website, a Linkedin, Twitter or Github profile…


####a <var>license</var> property####

The license which you prefer to release your project under. 

<code>MIT</code> is a good choice.

Each license is a hash with a "type" property specifying the type of license and a url property linking to the actual text.

```
	"license": {
		"type": "GPLv2",
		"url": "http://www.example.com/licenses/gpl.html"
	}
```

Alternatively, a single string may be provided.

If the license is one of the [official open source licenses](http://opensource.org/licenses/alphabetical) the official license name or its abbreviation may be explicated with the "type" property. If an abbreviation is provided (in parentheses), the abbreviation must be used.

```
	"license": "MIT"
```

If multiple licenses are applicable, they can be listed in an array.

```
	"licenses" : [
		{
			"type" : "Mozilla Public License 2.0 (MPL-2.0)", 
			"url" : "http://www.mozilla.org/MPL/2.0/"
		},
		{
			"type" : "MyLicense", 
			"url" : "http://github.com/owner/project/path/to/license"
		}
	]
```



## Legal Terms

By sending a "pull request" for the Directory and/or by using/downloading content available on the Directory, you agree to be bound by the following terms and conditions. 

###1. Grant of license

 By providing content and/or information for the Directory, you :

 * grant 4D and all the users of the Directory a worldwide, irrevocable, royalty-free, non-exclusive and unrestricted license to reproduce, edit, publish, translate, and distribute in any medium whatsoever. 
 * agree that 4D and all the users of the Directory can do all things in relation to your content and notably make a derivative work.
 * Agree that 4D can bundle your content in its Wakanda’s products.

###2. Warranties

 You represent and warrant that: (a) you are the author of such content and have the right to grant this license; (b) the content does not infringe any patent, copyright, trademark, trade secret or other proprietary right of any other party; and (c) no consent of any third party is necessary for exploiting your content as described above.

###3. Indemnification

 You shall indemnify, defend and hold harmless 4D and its subsidiaries from and against all liabilities, claims, demands, actions, costs, damages, or losses, including reasonable attorney's fees, initiated by or on behalf of third parties arising out of a claim that your content infringe such third party’s intellectual property rights. 

###4. Disclaimer 

 4D does not represent or endorse the accuracy or reliability of any of the information, content contained on, distributed through, or linked, downloaded or accessed from any of the services contained on this Directory nor the quality of any content or information displayed, or obtained by you. 

 The service, the content and the information herein are provided by 4D on an "as is" and “as available” basis, and 4D makes no warranty or representation (express or implied) of any kind, and 4d disclaims any and all other warranties, whether express or implied, including, without limitation, any implied warranties of merchantability, integration, satisfactory quality or fitness for a particular purpose.  Without limitation of the foregoing, 4d does not warrant that the content and/or information available on the Directory are free from bugs and/or errors and/or that the functions included in the Contents will meet user’s requirements. 

 The entire risk as to choice and use of the content and information available on this Directory is with the users of such contents.

 In no event shall 4D be liable for any direct, indirect, incidental, punitive, or consequential damages of any kind whatsoever with respect to the contents and the information available on this Directory.





