---
keywords: fastai
title: "Lists Quiz"
toc: true
branch: master
badges: true
comments: true
author: Dillon Lee
categories: [CSP Assignments, Week 3]
nb_path: _notebooks/2022-09-02-Lists Quiz.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-09-02-Lists Quiz.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">q1</span> <span class="o">=</span> <span class="s2">&quot;&quot;&quot;Which room is CSP in?</span>
<span class="s2">a. A101</span>
<span class="s2">b. A111</span>
<span class="s2">c. A115</span>
<span class="s2">d. D114&quot;&quot;&quot;</span>
<span class="n">q2</span> <span class="o">=</span> <span class="s2">&quot;&quot;&quot;Which teacher is the best teacher?</span>
<span class="s2">a. Mrs. Mansour</span>
<span class="s2">b. Mrs. Roberts</span>
<span class="s2">c. Mr. Yeung</span>
<span class="s2">d. I hate all teachers&quot;&quot;&quot;</span>
<span class="n">q3</span> <span class="o">=</span> <span class="s2">&quot;&quot;&quot;255+1534?</span>
<span class="s2">a. 1999</span>
<span class="s2">b. 1509</span>
<span class="s2">c. 1489</span>
<span class="s2">d. 1789&quot;&quot;&quot;</span>

<span class="n">questions</span> <span class="o">=</span> <span class="p">{</span><span class="n">q1</span> <span class="p">:</span> <span class="s2">&quot;a&quot;</span><span class="p">,</span><span class="n">q2</span> <span class="p">:</span> <span class="s2">&quot;c&quot;</span><span class="p">,</span><span class="n">q3</span> <span class="p">:</span> <span class="s2">&quot;d&quot;</span><span class="p">}</span>

<span class="n">name</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter your name: &quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Hello&quot;</span><span class="p">,</span><span class="n">name</span><span class="p">,</span> <span class="s2">&quot;welcome to the quiz world&quot;</span><span class="p">)</span>
<span class="n">score</span><span class="o">=</span><span class="mi">0</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">questions</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
    <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;enter the answer(a/b/c/d) : &quot;</span><span class="p">)</span>
    <span class="k">if</span> <span class="n">ans</span><span class="o">==</span><span class="n">questions</span><span class="p">[</span><span class="n">i</span><span class="p">]:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;correct answer, you got 1 point&quot;</span><span class="p">)</span>
        <span class="n">score</span> <span class="o">=</span> <span class="n">score</span><span class="o">+</span><span class="mi">1</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;wrong answer, you lost 1 point&quot;</span><span class="p">)</span>
        <span class="n">score</span><span class="o">=</span><span class="n">score</span><span class="o">-</span><span class="mi">1</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Final score is:&quot;</span><span class="p">,</span> <span class="n">score</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello Dillon welcome to the quiz world
Which room is CSP in?
a. A101
b. A111
c. A115
d. D114
correct answer, you got 1 point
Which teacher is the best teacher?
a. Mrs. Mansour
b. Mrs. Roberts
c. Mr. Yeung
d. I hate all teachers
correct answer, you got 1 point
255+1534?
a. 1999
b. 1509
c. 1489
d. 1789
wrong answer, you lost 1 point
Final score is: 1
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

