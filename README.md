[![pypi](https://badge.fury.io/py/pyglet.svg)](https://pypi.python.org/pypi/pyglet)

![logo_large.png](https://bitbucket.org/repo/aejyXX/images/3385888514-logo_large.png)

# pyglet

*pyglet* is a cross-platform windowing and multimedia library for Python, intended for developing games and other visually rich applications. It supports windowing, user interface event handling, Joysticks, OpenGL graphics, loading images and videos, and playing sounds and music. *pyglet* works on Windows, OS X and Linux.

* pyglet [documentation]
* pyglet [wiki]
* pyglet on [PyPI]
* pyglet [discord] server
* pyglet [mailing list]
* Pyglet [website]

Pyglet has an active developer and user community.  If you find a bug or issue, please [open an issue](https://github.com/pyglet/pyglet/issues).
Anyone is welcome to join our [discord] server were a lot
if the development discussion is going on. It's also a great place
to ask for help.

Some of the features of pyglet are:

* **No external dependencies or installation requirements.** For most application and game requirements, *pyglet* needs nothing else besides Python, simplifying distribution and installation. It's easy to package your project with freezers such as PyInstaller. 
* **Take advantage of multiple windows and multi-monitor desktops.** *pyglet* allows you to use multiple platform-native windows, and is fully aware of multi-monitor setups for use with fullscreen games.
* **Load images, sound, music and video in almost any format.** *pyglet* can optionally use FFmpeg to play back audio formats such as MP3, OGG/Vorbis and WMA, and video formats such as DivX, MPEG-2, H.264, WMV and Xvid. Without FFmpeg, *pyglet* contains built-in support for standard formats such as wav, png, bmp, and others.
* **pyglet is written entirely in pure Python**, and makes use of the *ctypes* module to interface with system libraries. You can modify the codebase or make a contribution without any second language compilation steps or compiler setup. Despite being pure Python, *pyglet* has excellent performance thanks to advanced batching for drawing thousands of sprites or animations.
* **pyglet is provided under the BSD open-source license**, allowing you to use it for both commercial and other open-source projects with very little restriction.

## Requirements

pyglet runs under Python 2.7, and 3.4+. The entire codebase is fully 2/3 dual
compatible, making use of the future module for backwards compatibility with
legacy Python. Being written in pure Python, it also works on other Python
interpreters such as PyPy. Supported platforms are:

* Windows XP or later
* Mac OS X 10.3 or later
* Linux, with the following libraries (most recent distributions will have
  these in a default installation):
  * OpenGL and GLX
  * GDK 2.0+ or PIL (required for loading images other than PNG and BMP)
  * OpenAL or Pulseaudio (required for playing audio)

**Please note that pyglet v1.4 will likely be the last version to support
Python 2.7**. Future releases of pyglet will be Python 3 only, and will be
targeting OpenGL 3.3+. Previous releases will remain available for download.

Starting with version 1.4, to play compressed audio and video files,
you will also need [FFmpeg](https://ffmpeg.org/).

## Installation

pyglet is installable from PyPI:

    pip install --upgrade pyglet --user

## Contributing

**A good way to start contributing to a component of pyglet is by its documentation**. When studying the code you are going to work with, also read the associated docs. If you don't understand the code with the help of the docs, it is a sign that the docs should be improved.

If you want to contribute to Pyglet, we suggest the following:

* Fork the [official repository](https://github.com/pyglet/pyglet/fork).
* Apply your changes to your fork.
* Submit a [pull request](https://github.com/pyglet/pyglet/pulls) describing the changes you have made.
* Alternatively you can create a patch and submit it to the issue tracker.

When making a pull request, check that you have addressed its respective documentation, both within the code docstrings and the programming guide (if applicable). It is very important to all of us that the documentation matches the latest code and vice-versa.

Consequently, an error in the documentation, either because it is hard to understand or because it doesn't match the code, is a bug that deserves to be reported on a ticket.

## Installation from source

If you're reading this `README` from a source distribution, you can install pyglet with:

    python setup.py install

You can also install the latest development version direct from Github using:

    pip install --upgrade https://github.com/pyglet/pyglet/archive/master.zip --user

For local development install pyglet in editable mode:

```bash
# with pip
pip install -e .
# with setup.py
python setup.py develop
```

There are no compilation steps during the installation; if you prefer,
you can simply add this directory to your `PYTHONPATH` and use pyglet without
installing it. You can also copy pyglet directly into your project folder.

## Building Docs

If you want to build the documentation yourself, please check
[the README file in the doc directory](doc/README).

## Testing

pyglet makes use of pytest for its test suite.

    pytest tests/

Please check the documentation for more information about running and writing tests.

# Contact

pyglet is developed by many individual volunteers, and there is no central point of contact. If you have a question about developing with pyglet, or you wish to contribute, please join the [mailing list] or the [discord] channel.

For legal issues, please contact [Alex Holkner](mailto:Alex.Holkner@gmail.com).

[discord]: https://discord.gg/QXyegWe
[mailing list]: http://groups.google.com/group/pyglet-users
[documentation]: https://pyglet.readthedocs.io
[wiki]:  https://github.com/pyglet/pyglet/wiki
[pypi]:  https://pypi.org/project/pyglet/
[website]: http://pyglet.org/
