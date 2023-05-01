---
keywords: fastai
title: "Variables and Assignment in JavaScript"
toc: true
branch: master
badges: true
comments: true
categories: [CSP Notes]
author: Dillon Lee
nb_path: _notebooks/2022-11-27-VariablesJavaScript.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-11-27-VariablesJavaScript.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Numbers"><strong>Numbers</strong><a class="anchor-link" href="#Numbers"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="kd">var</span> <span class="nx">x</span> <span class="o">=</span> <span class="mf">1</span><span class="p">;</span>
<span class="kd">var</span> <span class="nx">y</span> <span class="o">=</span> <span class="mf">2</span><span class="p">;</span>
<span class="kd">var</span> <span class="nx">z</span> <span class="o">=</span> <span class="nx">x</span> <span class="o">+</span> <span class="nx">y</span><span class="p">;</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">z</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>3
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
<div class=" highlight hl-javascript"><pre><span></span><span class="kr">const</span> <span class="nx">q</span> <span class="o">=</span> <span class="mf">5</span><span class="p">;</span>
<span class="kr">const</span> <span class="nx">w</span> <span class="o">=</span> <span class="mf">6</span><span class="p">;</span>
<span class="kd">let</span> <span class="nx">s</span> <span class="o">=</span> <span class="nx">q</span> <span class="o">+</span> <span class="nx">w</span><span class="p">;</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">s</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>11
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Boolean"><strong>Boolean</strong><a class="anchor-link" href="#Boolean"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="nb">Boolean</span><span class="p">(</span><span class="nx">w</span> <span class="o">&gt;</span> <span class="nx">q</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">



<div class="output_text output_subarea output_execute_result">
<pre>true</pre>
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
<div class=" highlight hl-javascript"><pre><span></span><span class="nb">Boolean</span><span class="p">(</span><span class="nx">w</span> <span class="o">&lt;</span> <span class="nx">q</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">



<div class="output_text output_subarea output_execute_result">
<pre>false</pre>
</div>

</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="String"><strong>String</strong><a class="anchor-link" href="#String"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="kd">let</span> <span class="nx">groupname</span> <span class="o">=</span> <span class="s2">&quot;ZestyYeungs&quot;</span><span class="p">;</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">groupname</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>ZestyYeungs
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="List"><strong>List</strong><a class="anchor-link" href="#List"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="kr">const</span> <span class="nx">groupnames</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Dillon&quot;</span><span class="p">,</span> <span class="s2">&quot;Rohan&quot;</span><span class="p">,</span> <span class="s2">&quot;Adi&quot;</span><span class="p">,</span> <span class="s2">&quot;Tay&quot;</span><span class="p">];</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">groupnames</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[ &#39;Dillon&#39;, &#39;Rohan&#39;, &#39;Adi&#39;, &#39;Tay&#39; ]
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
<div class=" highlight hl-javascript"><pre><span></span><span class="kr">const</span> <span class="nx">group</span> <span class="o">=</span> <span class="p">[</span>
    <span class="s2">&quot;Dillon&quot;</span><span class="p">,</span> 
    <span class="s2">&quot;Rohan&quot;</span><span class="p">,</span> 
    <span class="s2">&quot;Adi&quot;</span><span class="p">,</span> 
    <span class="s2">&quot;Tay&quot;</span>
<span class="p">];</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="nx">group</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[ &#39;Dillon&#39;, &#39;Rohan&#39;, &#39;Adi&#39;, &#39;Tay&#39; ]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 
