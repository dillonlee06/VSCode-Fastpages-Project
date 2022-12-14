---
keywords: fastai
description: "Bash bash bash"
title: "Bash Tutorial Check"
toc: true
branch: master
badges: true
comments: true
author: Dillon Lee
categories: [CSP Assignments, CSP Notes, Week 2]
nb_path: _notebooks/2022-08-25-Bash Tutorial.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-08-25-Bash Tutorial.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;Using conditional statement to create a project directory and project&quot;</span>
 
<span class="c1"># Variable section</span>
<span class="nb">export</span> <span class="nv">project_dir</span><span class="o">=</span><span class="nv">$HOME</span>/vscode  <span class="c1"># change vscode to different name to test git clone</span>
<span class="nb">export</span> <span class="nv">project</span><span class="o">=</span><span class="nv">$project_dir</span>/APCSP  <span class="c1"># change APCSP to name of project from git clone</span>
<span class="nb">export</span> <span class="nv">project_repo</span><span class="o">=</span><span class="s2">&quot;https://github.com/nighthawkcoders/APCSP.git&quot;</span>  <span class="c1"># change to project of choice</span>
 
<span class="nb">cd</span> ~    <span class="c1"># start in home directory</span>
 
<span class="c1"># Conditional block to make a project directory</span>
<span class="k">if</span> <span class="o">[</span> ! -d <span class="nv">$project_dir</span> <span class="o">]</span>
<span class="k">then</span>
   <span class="nb">echo</span> <span class="s2">&quot;Directory </span><span class="nv">$project_dir</span><span class="s2"> does not exists... makinng directory </span><span class="nv">$project_dir</span><span class="s2">&quot;</span>
   mkdir -p <span class="nv">$project_dir</span>
<span class="k">fi</span>
<span class="nb">echo</span> <span class="s2">&quot;Directory </span><span class="nv">$project_dir</span><span class="s2"> exists.&quot;</span>
 
<span class="c1"># Conditional block to git clone a project from project_repo</span>
<span class="k">if</span> <span class="o">[</span> ! -d <span class="nv">$project</span> <span class="o">]</span>
<span class="k">then</span>
   <span class="nb">echo</span> <span class="s2">&quot;Directory </span><span class="nv">$project</span><span class="s2"> does not exists... cloning </span><span class="nv">$project_repo</span><span class="s2">&quot;</span>
   <span class="nb">cd</span> <span class="nv">$project_dir</span>
   git clone <span class="nv">$project_repo</span>
   <span class="nb">cd</span> ~
<span class="k">fi</span>
<span class="nb">echo</span> <span class="s2">&quot;Directory </span><span class="nv">$project</span><span class="s2"> exists.&quot;</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Using conditional statement to create a project directory and project
Directory /Users/dillonlee/vscode exists.
Directory /Users/dillonlee/vscode/APCSP exists.
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;Navigate to project, then navigate to area wwhere files were cloned&quot;</span>
<span class="nb">cd</span> <span class="nv">$project</span>
<span class="nb">pwd</span>
 
<span class="nb">echo</span> <span class="s2">&quot;&quot;</span>
<span class="nb">echo</span> <span class="s2">&quot;list top level or root of files with project pulled from github&quot;</span>
ls
 
<span class="nb">echo</span> <span class="s2">&quot;&quot;</span>
<span class="nb">echo</span> <span class="s2">&quot;list again with hidden files pulled from github&quot;</span>
ls -a   <span class="c1"># hidden files flag, many shell commands have flags</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Navigate to project, then navigate to area wwhere files were cloned
/Users/dillonlee/vscode/APCSP

list top level or root of files with project pulled from github
Gemfile			_includes		_word
LICENSE			_layouts		assets
Makefile		_notebooks		docker-compose.yml
README.md		_pages			images
_action_files		_plugins		index.html
_config.yml		_posts			python
_fastpages_docs		_sass

list again with hidden files pulled from github
.			Makefile		_posts
..			README.md		_sass
.devcontainer.json	_action_files		_word
.git			_config.yml		assets
.gitattributes		_fastpages_docs		docker-compose.yml
.github			_includes		images
.gitignore		_layouts		index.html
.vscode			_notebooks		python
Gemfile			_pages
LICENSE			_plugins
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;&quot;</span>
<span class="nb">echo</span> <span class="s2">&quot;list all files in long format&quot;</span>
ls -al   <span class="c1"># all files and long listing</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>
list all files in long format
total 96
drwxr-xr-x  28 dillonlee  staff    896 Aug 23 15:23 .
drwxr-xr-x   3 dillonlee  staff     96 Aug 23 15:23 ..
-rw-r--r--   1 dillonlee  staff    420 Aug 23 15:23 .devcontainer.json
drwxr-xr-x  12 dillonlee  staff    384 Aug 23 15:23 .git
-rw-r--r--   1 dillonlee  staff     84 Aug 23 15:23 .gitattributes
drwxr-xr-x   4 dillonlee  staff    128 Aug 23 15:23 .github
-rw-r--r--   1 dillonlee  staff    917 Aug 23 15:23 .gitignore
drwxr-xr-x   3 dillonlee  staff     96 Aug 23 15:23 .vscode
-rwxr-xr-x   1 dillonlee  staff   1304 Aug 23 15:23 Gemfile
-rw-r--r--   1 dillonlee  staff  11351 Aug 23 15:23 LICENSE
-rwxr-xr-x   1 dillonlee  staff   1422 Aug 23 15:23 Makefile
-rwxr-xr-x   1 dillonlee  staff   3614 Aug 23 15:23 README.md
drwxr-xr-x  18 dillonlee  staff    576 Aug 23 15:23 _action_files
-rw-r--r--   1 dillonlee  staff   3716 Aug 23 15:23 _config.yml
drwxr-xr-x  24 dillonlee  staff    768 Aug 23 15:23 _fastpages_docs
drwxr-xr-x  29 dillonlee  staff    928 Aug 23 15:23 _includes
drwxr-xr-x   6 dillonlee  staff    192 Aug 23 15:23 _layouts
drwxr-xr-x  11 dillonlee  staff    352 Aug 23 15:23 _notebooks
drwxr-xr-x   9 dillonlee  staff    288 Aug 23 15:23 _pages
drwxr-xr-x   4 dillonlee  staff    128 Aug 23 15:23 _plugins
drwxr-xr-x  29 dillonlee  staff    928 Aug 23 15:23 _posts
drwxr-xr-x   3 dillonlee  staff     96 Aug 23 15:23 _sass
drwxr-xr-x   3 dillonlee  staff     96 Aug 23 15:23 _word
drwxr-xr-x   4 dillonlee  staff    128 Aug 23 15:23 assets
-rwxr-xr-x   1 dillonlee  staff   1136 Aug 23 15:23 docker-compose.yml
drwxr-xr-x  52 dillonlee  staff   1664 Aug 23 15:23 images
-rw-r--r--   1 dillonlee  staff   1061 Aug 23 15:23 index.html
drwxr-xr-x   3 dillonlee  staff     96 Aug 23 15:23 python
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;Look for posts&quot;</span>
<span class="nb">export</span> <span class="nv">posts</span><span class="o">=</span><span class="nv">$project</span>/_posts  <span class="c1"># _posts inside project</span>
<span class="nb">cd</span> <span class="nv">$posts</span>  <span class="c1"># this should exist per fastpages</span>
<span class="nb">pwd</span>  <span class="c1"># present working directory</span>
ls -l  <span class="c1"># list posts</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Look for posts
/Users/dillonlee/vscode/APCSP/_posts
total 456
-rw-r--r--  1 dillonlee  staff  21306 Aug 23 15:23 2022-06-01-TT160-deploy.md
-rw-r--r--  1 dillonlee  staff   5861 Aug 23 15:23 2022-07-07-PBL-binary.md
-rw-r--r--  1 dillonlee  staff   3085 Aug 23 15:23 2022-07-08-PBL-grade_calc.md
-rw-r--r--  1 dillonlee  staff   3698 Aug 23 15:23 2022-07-08-PBL-graph.md
-rw-r--r--  1 dillonlee  staff   5729 Aug 23 15:23 2022-07-08-PBL-life.md
-rw-r--r--  1 dillonlee  staff  14387 Aug 23 15:23 2022-07-08-PBL-snake.md
-rw-r--r--  1 dillonlee  staff    334 Aug 23 15:23 2022-07-10-PBL-database.md
-rw-r--r--  1 dillonlee  staff   2908 Aug 23 15:23 2022-07-10-PBL-jokes.md
-rw-r--r--  1 dillonlee  staff   4046 Aug 23 15:23 2022-07-10-PBL-rapidapi.md
-rw-r--r--  1 dillonlee  staff   6685 Aug 23 15:23 2022-07-19-PBL-calculator.md
-rw-r--r--  1 dillonlee  staff  23325 Aug 23 15:23 2022-07-25-CSP-workshop.md
-rw-r--r--  1 dillonlee  staff   2333 Aug 23 15:23 2022-08-15-TP000-student_score_history.md
-rw-r--r--  1 dillonlee  staff   4363 Aug 23 15:23 2022-08-15-TP100-pseudo_code.md
-rw-r--r--  1 dillonlee  staff   7968 Aug 23 15:23 2022-08-15-TR100-tool_setup.md
-rw-r--r--  1 dillonlee  staff  15026 Aug 23 15:23 2022-08-15-TT100-tools.md
-rw-r--r--  1 dillonlee  staff   5590 Aug 23 15:23 2022-08-15-TT101-vscode-wsl.md
-rw-r--r--  1 dillonlee  staff   2155 Aug 23 15:23 2022-08-22-TR110-intro_python.md
-rw-r--r--  1 dillonlee  staff   5173 Aug 23 15:23 2022-08-22-TT110-fastpages.md
-rw-r--r--  1 dillonlee  staff   2798 Aug 23 15:23 2022-08-22-TT110-focus.md
-rw-r--r--  1 dillonlee  staff   2737 Aug 23 15:23 2022-08-29-TR120-data_abstract.md
-rw-r--r--  1 dillonlee  staff  10683 Aug 23 15:23 2022-08-29-TT120-agile.md
-rw-r--r--  1 dillonlee  staff   4498 Aug 23 15:23 2022-08-29-TT120-html_fragments.md
-rw-r--r--  1 dillonlee  staff   9037 Aug 23 15:23 2022-09-05-TP130-create_performance_task.md
-rw-r--r--  1 dillonlee  staff   7753 Aug 23 15:23 2022-09-05-TP131-create-task-bria.md
-rw-r--r--  1 dillonlee  staff   8066 Aug 23 15:23 2022-09-05-TR130-creative_development.md
-rw-r--r--  1 dillonlee  staff   3520 Aug 23 15:23 2022-09-05-TT130-applab.md
-rw-r--r--  1 dillonlee  staff    720 Aug 23 15:23 README.md
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;Look for notebooks&quot;</span>
<span class="nb">export</span> <span class="nv">notebooks</span><span class="o">=</span><span class="nv">$project</span>/_notebooks  <span class="c1"># _notebooks is inside project</span>
<span class="nb">cd</span> <span class="nv">$notebooks</span>   <span class="c1"># this should exist per fastpages</span>
<span class="nb">pwd</span>  <span class="c1"># present working directory</span>
ls -l  <span class="c1"># list notebooks</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Look for notebooks
/Users/dillonlee/vscode/APCSP/_notebooks
total 208
-rw-r--r--  1 dillonlee  staff  14243 Aug 23 15:23 2022-06-01-TT150-webapi_tutorial.ipynb
-rw-r--r--  1 dillonlee  staff   8653 Aug 23 15:23 2022-07-21-PBL-neo4j_intro.ipynb
-rw-r--r--  1 dillonlee  staff  11694 Aug 23 15:23 2022-08-22-TP110-python_hello.ipynb
-rw-r--r--  1 dillonlee  staff  20003 Aug 23 15:23 2022-08-22-TT110-anthony_and_sahil.ipynb
-rw-r--r--  1 dillonlee  staff   9525 Aug 23 15:23 2022-08-22-TT110-bash_tutorial.ipynb
-rw-r--r--  1 dillonlee  staff  10141 Aug 23 15:23 2022-08-29-TP120-python_lists.ipynb
-rw-r--r--  1 dillonlee  staff  12632 Aug 23 15:23 2022-09-05-TT130-js_tutorial.ipynb
-rw-r--r--  1 dillonlee  staff    771 Aug 23 15:23 README.md
drwxr-xr-x  3 dillonlee  staff     96 Aug 23 15:23 images
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;Look for images in notebooks, print working directory, list files&quot;</span>
<span class="nb">cd</span> <span class="nv">$notebooks</span>/images  <span class="c1"># this should exist per fastpages</span>
<span class="nb">pwd</span>
ls -l
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Look for images in notebooks, print working directory, list files
/Users/dillonlee/vscode/APCSP/_notebooks/images
total 200
-rw-r--r--  1 dillonlee  staff  101617 Aug 23 15:23 kernels.png
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;Navigate to project, then navigate to area wwhere files were cloned&quot;</span>
 
<span class="nb">cd</span> <span class="nv">$project</span>
<span class="nb">echo</span> <span class="s2">&quot;show the contents of README.md&quot;</span>
<span class="nb">echo</span> <span class="s2">&quot;&quot;</span>
 
cat README.md  <span class="c1"># show contents of file, in this case markdown</span>
<span class="nb">echo</span> <span class="s2">&quot;&quot;</span>
<span class="nb">echo</span> <span class="s2">&quot;end of README.md&quot;</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Navigate to project, then navigate to area wwhere files were cloned
show the contents of README.md

[//]: # (This template replaces README.md when someone creates a new repo with the fastpages template.)

![](https://github.com/nighthawkcoders/APCSP/workflows/CI/badge.svg) 
![](https://github.com/nighthawkcoders/APCSP/workflows/GH-Pages%20Status/badge.svg) 
[![](https://img.shields.io/static/v1?label=fastai&amp;message=fastpages&amp;color=57aeac&amp;labelColor=black&amp;style=flat&amp;logo=data:image/png;base64,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)](https://github.com/fastai/fastpages)

https://nighthawkcoders.github.io/APCSP/

# My Blog


_powered by [fastpages](https://github.com/fastai/fastpages)_


## What To Do Next?

Great!  You have setup your repo.  Now its time to start writing content.  Some helpful links:

- [Writing Blogs With Jupyter](https://github.com/fastai/fastpages#writing-blog-posts-with-jupyter)

- [Writing Blogs With Markdown](https://github.com/fastai/fastpages#writing-blog-posts-with-markdown)

- [Writing Blog Posts With Word](https://github.com/fastai/fastpages#writing-blog-posts-with-microsoft-word)

- [(Optional) Preview Your Blog Locally](_fastpages_docs/DEVELOPMENT.md)

Note: you may want to remove example blog posts from the `_posts`,  `_notebooks` or `_word` folders (but leave them empty, don&#39;t delete these folders) if you don&#39;t want these blog posts to appear on your site.

Please use the [nbdev &amp; blogging channel](https://forums.fast.ai/c/fastai-users/nbdev/48) in the fastai forums for any questions or feature requests.

end of README.md
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">echo</span> <span class="s2">&quot;Show the shell environment variables, key on left of equal value on right&quot;</span>
<span class="nb">echo</span> <span class="s2">&quot;&quot;</span>
 
env
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Show the shell environment variables, key on left of equal value on right

MANPATH=/opt/homebrew/share/man::
SHELL=/bin/zsh
HOMEBREW_REPOSITORY=/opt/homebrew
TMPDIR=/var/folders/1c/5fmmmphn2r5_sg3_vzbl9lgc0000gn/T/
CONDA_SHLVL=1
PYTHONUNBUFFERED=1
CONDA_PROMPT_MODIFIER=(base) 
OLDPWD=/Users/dillonlee/vscode/APCSP/_notebooks/images
ORIGINAL_XDG_CURRENT_DESKTOP=undefined
MallocNanoZone=0
PYTHONIOENCODING=utf-8
USER=dillonlee
COMMAND_MODE=unix2003
CONDA_EXE=/Users/dillonlee/opt/anaconda3/bin/conda
SSH_AUTH_SOCK=/private/tmp/com.apple.launchd.7IgjpJF2wZ/Listeners
__CF_USER_TEXT_ENCODING=0x1F5:0x0:0x0
JPY_PARENT_PID=60302
PAGER=cat
VSCODE_AMD_ENTRYPOINT=vs/workbench/api/node/extensionHostProcess
ELECTRON_RUN_AS_NODE=1
JUPYTER_PATH=/Users/dillonlee/.vscode/extensions/ms-toolsai.jupyter-2022.7.1102252217/temp/jupyter
_CE_CONDA=
PATH=/Users/dillonlee/opt/anaconda3/bin:/Users/dillonlee/opt/anaconda3/condabin:/opt/homebrew/bin:/opt/homebrew/sbin:/Library/Frameworks/Python.framework/Versions/2.7/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
CONDA_PREFIX=/Users/dillonlee/opt/anaconda3
__CFBundleIdentifier=com.microsoft.VSCode
PWD=/Users/dillonlee/vscode/APCSP
notebooks=/Users/dillonlee/vscode/APCSP/_notebooks
VSCODE_HANDLES_UNCAUGHT_ERRORS=true
project_repo=https://github.com/nighthawkcoders/APCSP.git
project=/Users/dillonlee/vscode/APCSP
project_dir=/Users/dillonlee/vscode
XPC_FLAGS=0x0
PS1=[PEXP\[\]ECT_PROMPT&gt;
_CE_M=
XPC_SERVICE_NAME=0
SHLVL=1
HOME=/Users/dillonlee
APPLICATION_INSIGHTS_NO_DIAGNOSTIC_CHANNEL=1
VSCODE_NLS_CONFIG={&#34;locale&#34;:&#34;en-us&#34;,&#34;availableLanguages&#34;:{},&#34;_languagePackSupport&#34;:true}
HOMEBREW_PREFIX=/opt/homebrew
PYTHONPATH=/Users/dillonlee/.vscode/extensions/ms-toolsai.jupyter-2022.7.1102252217/pythonFiles:/Users/dillonlee/.vscode/extensions/ms-toolsai.jupyter-2022.7.1102252217/pythonFiles/lib/python
CONDA_PYTHON_EXE=/Users/dillonlee/opt/anaconda3/bin/python
LOGNAME=dillonlee
LC_CTYPE=UTF-8
VSCODE_IPC_HOOK=/Users/dillonlee/Library/Application Support/Code/1.70.2-main.sock
VSCODE_CODE_CACHE_PATH=/Users/dillonlee/Library/Application Support/Code/CachedData/e4503b30fc78200f846c62cf8091b76ff5547662
CONDA_DEFAULT_ENV=base
VSCODE_PID=53351
posts=/Users/dillonlee/vscode/APCSP/_posts
INFOPATH=/opt/homebrew/share/info:
HOMEBREW_CELLAR=/opt/homebrew/Cellar
VSCODE_CWD=/
_=/usr/bin/env
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-bash"><pre><span></span><span class="nb">cd</span> <span class="nv">$project</span>
 
<span class="nb">echo</span> <span class="s2">&quot;&quot;</span>
<span class="nb">echo</span> <span class="s2">&quot;show the secrets of .git&quot;</span>
<span class="nb">cd</span> .git
ls -l
 
<span class="nb">echo</span> <span class="s2">&quot;&quot;</span>
<span class="nb">echo</span> <span class="s2">&quot;look at config file&quot;</span>
cat config
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>
show the secrets of .git
total 72
-rw-r--r--   1 dillonlee  staff     23 Aug 23 15:23 HEAD
-rw-r--r--   1 dillonlee  staff    314 Aug 23 15:23 config
-rw-r--r--   1 dillonlee  staff     73 Aug 23 15:23 description
drwxr-xr-x  15 dillonlee  staff    480 Aug 23 15:23 hooks
-rw-r--r--   1 dillonlee  staff  19916 Aug 23 15:23 index
drwxr-xr-x   3 dillonlee  staff     96 Aug 23 15:23 info
drwxr-xr-x   4 dillonlee  staff    128 Aug 23 15:23 logs
drwxr-xr-x   4 dillonlee  staff    128 Aug 23 15:23 objects
-rw-r--r--   1 dillonlee  staff    271 Aug 23 15:23 packed-refs
drwxr-xr-x   5 dillonlee  staff    160 Aug 23 15:23 refs

look at config file
[core]
	repositoryformatversion = 0
	filemode = true
	bare = false
	logallrefupdates = true
	ignorecase = true
	precomposeunicode = true
[remote &#34;origin&#34;]
	url = https://github.com/nighthawkcoders/APCSP.git
	fetch = +refs/heads/*:refs/remotes/origin/*
[branch &#34;master&#34;]
	remote = origin
	merge = refs/heads/master
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

