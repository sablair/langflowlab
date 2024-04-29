## The setup

LangFlow is truly awesome and it's so easy to get started. If you want to get up and going quickly, here's one way to go (this is written from the POV of someone who typically does not do much if any python).

At the time of this writing, to use the pre-release version of Langflow required that Python 3.10 is installed. My recommendation, install and configure [pyenv](https://github.com/pyenv/pyenv#installation). Afterwards, use pyenv to download and install the version of [Python](https://www.python.org/downloads/) you wish to use.

```bash
$ pyenv install 3.10.14
```

Once the version of python you need has been installed, select this version for usage. As I am running this locally, I chose to use the pyenv local command to automatically select this version of python whenever I am in this project's directory:

```bash
$ pyenv local 3.10.14
$ python3 -V
```

That last command is to confirm that I am using my stated version of Python.

I (now) try to always use a virtual environment to ensure reproducibility. So on that note:

```bash
$ python3 -m venv .venv
$ source .venv/bin/activate
```

Now we are ready to install [Langflow](https://github.com/langflow-ai/langflow). Note, that I am installing the **pre-release version**.

```bash
$ python3 -m pip install langflow --pre --force-reinstall
```

and after waiting a bit...

```bash
$ python3 -m langflow run
```

### Next steps

I watched this [video](https://youtu.be/RWo4GDTZIsE?si=ZbePNl5cYZKAXgca) and the very next day I created a proof of concept for a Q and A type chat bot based on the information available on our company's site. The hardest part was the initial set up but 15 minutes later gold!
