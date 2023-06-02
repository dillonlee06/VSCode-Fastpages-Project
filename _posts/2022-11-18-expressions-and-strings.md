---
keywords: fastai
description: Lesson on Big Idea 3 which includes expressions, strings, psuedocode, and more!
title: Unit 3.3, 3.4 Expressions and Strings Notes
toc: true
branch: master
badges: true
comments: true
author: Dillon Lee
categories: [CSP Notes, Presentation Notes]
nb_path: _notebooks/2022-11-18-expressions-and-strings.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-11-18-expressions-and-strings.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="3.3-Expressions(Show-video-1-and-3)">3.3 Expressions(Show video 1 and 3)<a class="anchor-link" href="#3.3-Expressions(Show-video-1-and-3)"> </a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Vocab:-fill-in-the-blanks">Vocab: fill in the blanks<a class="anchor-link" href="#Vocab:-fill-in-the-blanks"> </a></h3><p>the symbol for exponent is *<em><br>
the symbol for addition is <strong> + </strong><br>
the symbol for subtraction is <strong> - </strong><br>
the symbol for multiplication is __ </em> <strong><br>
the symbol for division is </strong> / <strong><br>
the symbol for modulus is </strong> % <strong><br>
an algorithm is </strong> a series of operations that completes a task/solves a problem __</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Sequencing Practice: the code below does not follow the intended steps below. change the code so that it does so.</p>
<ol>
<li>divide value1 by 10(value1 = 5)  </li>
<li>multiply 2 from the result of the step 1  </li>
<li>subtract 4 from the result of the step 2</li>
<li>print the result of step 3</li>
</ol>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">value1</span> <span class="o">=</span> <span class="mi">5</span>
<span class="n">value2</span> <span class="o">=</span> <span class="n">value1</span> <span class="o">/</span> <span class="mi">10</span> <span class="c1">#step 1</span>
<span class="n">value3</span> <span class="o">=</span> <span class="n">value2</span> <span class="o">*</span> <span class="mi">2</span> <span class="c1">#step 2</span>
<span class="n">value4</span> <span class="o">=</span> <span class="n">value3</span> <span class="o">-</span> <span class="mi">4</span> <span class="c1">#step 3</span>
<span class="nb">print</span><span class="p">(</span><span class="n">value4</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>-3.0
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Selection/Iteration Practice: Create a function to print ONLY the numbers of numlist that are divisble by 3.<br>
Hint: use the MOD operator (a % b) to find the remainder when a is divided by b.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">numlist</span> <span class="o">=</span> <span class="s2">&quot;3&quot;</span><span class="p">,</span><span class="s2">&quot;4&quot;</span><span class="p">,</span><span class="s2">&quot;9&quot;</span><span class="p">,</span><span class="s2">&quot;76&quot;</span><span class="p">,</span><span class="s2">&quot;891&quot;</span>
<span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">numlist</span><span class="p">:</span>
    <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="o">%</span> <span class="mi">3</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">num</span> <span class="o">+</span> <span class="s2">&quot; is divisible by 3&quot;</span><span class="p">)</span>
        <span class="k">continue</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">num</span> <span class="o">+</span> <span class="s2">&quot; is not divisible by 3&quot;</span><span class="p">)</span>
        <span class="k">continue</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>3 is divisible by 3
4 is not divisible by 3
9 is divisible by 3
76 is not divisible by 3
891 is divisible by 3
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Homework/Binary Adaptation: Create a python function that will convert a decimal number 1-255 to binary using mathematical operations and powers of 2. Challenge: add frontend with javascript or html.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">convert</span><span class="p">(</span><span class="n">num</span><span class="p">):</span> <span class="c1">#defines the variable and convert(x) function</span>
    <span class="n">result</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span> <span class="c1">#&quot;&quot; = what will be printed </span>
    <span class="n">i</span> <span class="o">=</span> <span class="mi">7</span>
    <span class="k">while</span> <span class="p">(</span><span class="mi">256</span> <span class="o">&gt;</span> <span class="n">i</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">):</span> <span class="c1"># creates the while loop which determines whether the number is even or odd and assign the binary 1 or 0s for the final print</span>
        <span class="k">if</span> <span class="n">num</span> <span class="o">%</span> <span class="p">(</span><span class="mi">2</span><span class="o">**</span><span class="n">i</span><span class="p">)</span> <span class="o">==</span> <span class="n">num</span><span class="p">:</span> 
            <span class="n">result</span> <span class="o">=</span> <span class="n">result</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
            <span class="n">i</span> <span class="o">-=</span> <span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="n">result</span> <span class="o">=</span> <span class="n">result</span> <span class="o">+</span> <span class="s2">&quot;1&quot;</span>
            <span class="n">num</span> <span class="o">-=</span> <span class="mi">2</span><span class="o">**</span><span class="n">i</span>
            <span class="n">i</span> <span class="o">-=</span> <span class="mi">1</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">result</span><span class="p">)</span> <span class="c1"># print the result defined in line 2</span>
<span class="n">convert</span><span class="p">(</span><span class="mi">66</span><span class="p">)</span> <span class="c1"># conversion from line 1</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>0100001
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="3.4-Strings(Show-video-1)">3.4 Strings(Show video 1)<a class="anchor-link" href="#3.4-Strings(Show-video-1)"> </a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Vocab:-fill-in-the-blanks-using-the-video">Vocab: fill in the blanks using the video<a class="anchor-link" href="#Vocab:-fill-in-the-blanks-using-the-video"> </a></h3><p>Index is a number representing a position, like a character's position in a string or a string's position in a list.<br>
Concatenation is <strong> combination of strings </strong> 
Length is <strong> number of characters in the string </strong><br>
A substring is <strong>_ part of a string __</strong></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="What-is-psuedocode?">What is psuedocode?<a class="anchor-link" href="#What-is-psuedocode?"> </a></h3><p>Pseudocode is writing out a program in plain language with keywords that are used to refer to common coding concepts.</p>
<p>Can you think of some benefits of using pseudocode prior to writing out the actual code?</p>
<ol>
<li>Choose an everyday activity</li>
<li>Imagine that you are providing instructions for this activity to a person who has never done it before</li>
<li>Challenge someone to do the steps you wrote out</li>
</ol>
<p>Ex. Brushing Teeth</p>
<ol>
<li>Pick up your toothbrush</li>
<li>Rinse toothbrush</li>
<li>Pick up toothpaste</li>
<li>Place toothpaste on the toothbrush</li>
<li>Rinse toothbrush again</li>
<li>Brush teeth in a circular motion</li>
<li>Spit</li>
<li>Wash mouth </li>
<li>Rinse toothbrush</li>
<li>You have brushed your teeth!</li>
</ol>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Substring/Length-Practice:-change-the-print-functions-to-print-&quot;hello&quot;,-&quot;bye&quot;,-and-the-string-length">Substring/Length Practice: change the print functions to print "hello", "bye", and the string length<a class="anchor-link" href="#Substring/Length-Practice:-change-the-print-functions-to-print-&quot;hello&quot;,-&quot;bye&quot;,-and-the-string-length"> </a></h3>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#the substring will have the characters including the index &quot;start&quot; to the character BEFORE the index &quot;end&quot;</span>
<span class="c1">#len(string) will print the length of string</span>

<span class="n">string</span> <span class="o">=</span> <span class="s2">&quot;hellobye&quot;</span>
<span class="n">x</span> <span class="o">=</span> <span class="n">string</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">8</span><span class="p">]</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">string</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">5</span><span class="p">]</span>
<span class="n">z</span> <span class="o">=</span> <span class="n">string</span><span class="p">[</span><span class="mi">5</span><span class="p">:</span><span class="mi">8</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">string</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="n">y</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">z</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>hellobye
8
hello
bye
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Concatenation Practice: combine string1 and string2 to make string3, then print string3.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">string1</span> <span class="o">=</span> <span class="s2">&quot;computer&quot;</span>
<span class="n">string2</span> <span class="o">=</span> <span class="s2">&quot;science&quot;</span>
<span class="n">string3</span> <span class="o">=</span> <span class="n">string1</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span> <span class="o">+</span> <span class="n">string2</span>
<span class="nb">print</span><span class="p">(</span><span class="n">string3</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>computer science
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Homework/List Adaptation: create a function that prints the name of each string in the list and the string's length. Challenge: add frontend with javascript or html.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">names</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;jaden&quot;</span><span class="p">,</span><span class="s2">&quot;max&quot;</span><span class="p">,</span><span class="s2">&quot;dylan&quot;</span><span class="p">,</span><span class="s2">&quot;orlando&quot;</span><span class="p">]</span>

<span class="k">def</span> <span class="nf">length</span><span class="p">(</span><span class="nb">list</span><span class="p">):</span>
    <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span> <span class="c1">#calls the strings in the list of names</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">x</span> <span class="o">+</span> <span class="s2">&quot; = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">x</span><span class="p">)))</span> <span class="c1">#prints the output &quot;name&quot; = the length (int) converted into a string</span>
        
<span class="n">length</span><span class="p">(</span><span class="n">names</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>jaden = 5
max = 3
dylan = 5
orlando = 7
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Stuck?">Stuck?<a class="anchor-link" href="#Stuck?"> </a></h1><ul>
<li>Check out <a href="https://raisinbran25.github.io/csp2/2022/11/18/expressions.html">what we did.</a></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Have-any-questions?">Have any questions?<a class="anchor-link" href="#Have-any-questions?"> </a></h1><ul>
<li>Ask us if you have any questions!</li>
</ul>

</div>
</div>
</div>
</div>
 
