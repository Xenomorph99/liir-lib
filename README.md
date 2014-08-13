Лийр Library
============
A pear flavored SCSS library.

Installation
------------
1. Create a new directory called `lib` inside your SCSS directory.  (You can call the new directory anything you want just make sure you're consistant.)

	```bash
	$ cd yoursite.com/scss/
	$ mkdir lib
	$ cd lib
	```

2. Initalize git and clone this repo into the new `lib` directory.

	```bash
	$ git init
	$ git remote add origin git@github.com:Alekhen/liir-lib.git
	$ git fetch
	$ git checkout -t origin/master
	```

3. Copy the `_variables.scss` file from the library into the parent directory and rename it as `_lib-config.scss`.  File name and location are important here since the Лийр Library will need to access this file.  `_lib-config.scss` is where you can customize the library's compiled output by overwriting the default variables.

	```bash
	$ cp _variables.scss ../_lib-config.scss
	```

4. Include the `lib/_liir.scss` file in your project and you're good to go.

	```scss
	@import "lib/liir";
	```

5. _Optional:_ If you ONLY want access to Лийр's mixin library you can choose to include `lib/mixins/_config.scss` instead of `lib/_liir.scss` in your project.

	```scss
	@import "lib/mixins/config";
	```

6. _Optional:_ Add the `lib` directory to your `.gitignore` file if you don't want the Лийр Library to be stored in your project repo.


Change Log
----------
### v1.0 - Current Version


License
-------
Copyright © 2014, [Hazard Media Group LLC](http://hazardmediagroup.com)

* [MIT License](https://github.com/Alekhen/intoor/blob/master/LICENSE)


Development
-----------
* Source hosted at [GitHub](https://github.com/Alekhen/liir-lib).

#### Author
[Colton James Wiscombe](http://coltonjameswiscombe.com)