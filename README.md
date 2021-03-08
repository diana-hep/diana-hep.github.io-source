# diana-hep.github.io-source
pelican source for website

![](https://travis-ci.org/diana-hep/diana-hep.github.io-source.svg?branch=master)


Created DIANA-HEP GitHub Organization
Using [Pelican](http://getpelican.com/) to generate website with fork of [pelican-bootsrap3](https://github.com/diana-hep/pelican-bootstrap3) theme

Using Travis to build website -- [how-to](http://zonca.github.io/2013/09/automatically-build-pelican-and-publish-to-github-pages.html)



For local testing:

```bash
# Make a local venv
python3 -m venv venv

# Activate the venv (redo this if you restart the terminal)
source venv/bin/activate

# Install the nice requirements
pip install -r requirements.txt

# Install the hacky requirements (should be submodules, but I digress)
git clone https://github.com/diana-hep/pelican-bootstrap3.git
git clone --recursive https://github.com/getpelican/pelican-plugins
git clone https://github.com/michael-milette/Tipue-Search
cp -r Tipue-Search/tipuesearch pelican-bootstrap3/static/

# Build and serve
make html
make serve
```

When you are done, run `deactivate` to leave the virtual environment.

