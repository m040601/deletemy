https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2


HTML Tags You Can Use on GitHub

Wherever HTML is rendered on GitHub (gists, README files in repos, comments on issues and pull requests, ...) you can use any of the HTML elements that GitHub Flavored Markdown (GFM) provides syntactic sugar for. You can either use the syntactic sugar that GFM (or other GitHub-supported markup language you're using) provides or, since Markdown can contain raw HTML, you can enter the HTML tags manually.

But GitHub also allows you to use a few HTML elements beyond what Markdown provides by entering the tags manually, and some of them are styled with CSS. Most raw HTML tags get stripped before rendering the HTML. Those tags that can be generated by GFM syntactic sugar, plus a few more, are whitelisted. These aren't documented anywhere that I can find. Here's what I've discovered so far:





# trying out only the 'pre' block

<pre>
<span style="font-weight:bold;color:#af875f;">[1988] Yoko Nagayama – F1 [Full Album] [4EcItfthCFA].m4a</span>
<span style="color:#008787;">aurydesty</span>
<span style="font-weight:bold;color:#af005f;">l.html</span>
<span style="font-weight:bold;color:#af005f;">lnohead.html</span>
<span style="font-weight:bold;color:#af005f;">ls.html</span>
<span style="color:#d7ff00;">newsboat_error.log</span>
<span style="color:#e0e0e0;">tmux_copy.txt</span>
</pre>


# pre block without pre tags

<span style="font-weight:bold;color:#af875f;">[1988] Yoko Nagayama – F1 [Full Album] [4EcItfthCFA].m4a</span>
<span style="color:#008787;">aurydesty</span>
<span style="font-weight:bold;color:#af005f;">l.html</span>
<span style="font-weight:bold;color:#af005f;">lnohead.html</span>
<span style="font-weight:bold;color:#af005f;">ls.html</span>
<span style="color:#d7ff00;">newsboat_error.log</span>
<span style="color:#e0e0e0;">tmux_copy.txt</span>


# a details and summary block

<details open>
  <summary>This is the summary</summary>
  <p>And here are the details:</p>
  <ol>
    <li>Cash on hand: $500.00</li>
    <li>Current invoice: $75.30</li>
    <li>Due date: 5/6/19</li>
  </ol>
</details>






# Try putting your HTML snippet inside an ```HTML block like this:

```html
<h2>Example of code</h2>

<pre>
    <div class="container">
        <div class="block two first">
            <h2>Your title</h2>
            <div class="wrap">
            //Your content
            </div>
        </div>
    </div>
</pre>
```






# w3c html5 kbd, samp

https://iandevlin.com/blog/2012/07/html5/using-html-kbd-samp-and-pre-elements/

As the name might suggest, the kbd element is used to represent user input that is typically entered via a keyboard. You might use this when you are describing what a user would enter to carry out a specific task, for example:



```
To get a list of directories, type <kbd>dir</kbd> in the command line and press <kbd>Enter</kbd>
```

To get a list of directories, type <kbd>dir</kbd> in the command line and press <kbd>Enter</kbd>



```
It wasn't the most helpful of <samp>error messages</samp> as it simply said: <samp>An error has occurred</samp>.
```

It wasn't the most helpful of <samp>error messages</samp> as it simply said: <samp>An error has occurred</samp>.



```
<pre><samp>C:\\></samp>
<kbd><kbd>cd html5</kbd> + <kbd>Enter</kbd></kbd>
<samp>C:\\html5></samp></pre>
```

<pre><samp>C:\\></samp>
<kbd><kbd>cd html5</kbd> + <kbd>Enter</kbd></kbd>
<samp>C:\\html5></samp></pre>



```
<code><p>After typing in <kbd>cd D:</kbd> at the command prompt, the output should show <samp>D:\></samp></p></code>
```

<code><p>After typing in <kbd>cd D:</kbd> at the command prompt, the output should show <samp>D:\></samp></p></code>

or


```
<code><pre><code>void main(void) {}</code></pre></code>
```

<code><pre><code>void main(void) {}</code></pre></code>






# HTML Tags You Can Use on GitHub



```
<details open>
  <summary>This is the summary</summary>
  <p>And here are the details:</p>
  <ol>
    <li>Cash on hand: $500.00</li>
    <li>Current invoice: $75.30</li>
    <li>Due date: 5/6/19</li>
  </ol>
</details>
```



<details open>
  <summary>This is the summary</summary>
  <p>And here are the details:</p>
  <ol>
    <li>Cash on hand: $500.00</li>
    <li>Current invoice: $75.30</li>
    <li>Due date: 5/6/19</li>
  </ol>
</details>


```
<pre><samp>mike@interwebz:~$ <kbd>md5 -s "Hello world"</kbd>
MD5 ("Hello world") = 3e25960a79dbc69b674cd4ec67a72c62

mike@interwebz:~$ █</samp></pre>
```


<pre><samp>mike@interwebz:~$ <kbd>md5 -s "Hello world"</kbd>
MD5 ("Hello world") = 3e25960a79dbc69b674cd4ec67a72c62

mike@interwebz:~$ █</samp></pre>

```
Subscripts<sub>sub</sub> and superscripts<sup>sup</sup> with `<sub>` and `<sup>`.
```

Subscripts<sub>sub</sub> and superscripts<sup>sup</sup> with `<sub>` and `<sup>`.



```
You can use `<sup>` to create linked footnotes.<sup id="backToMyFootnote"><a href="#myFootnote">1</a></sup>
```

You can use `<sup>` to create linked footnotes.<sup id="backToMyFootnote"><a href="#myFootnote">1</a></sup>


```
Inserted text with `<ins>`: <ins>inserted</ins> and deleted text with `<del>`: <del>deleted</del>. These can both have the `cite` attribute.
```


Inserted text with `<ins>`: <ins>inserted</ins> and deleted text with `<del>`: <del>deleted</del>. These can both have the `cite` attribute.


```
Variables with `<var>`: <var>myVariable</var>.
```

Variables with `<var>`: <var>myVariable</var>.


```
Inline quotes with `<q>` get curly quotation marks around them: <q>inline quote</q>. You can also use the `cite` attribute on them. You can use `cite` on a `<blockquote>` too, if you enter the `<blockquote>` manually.
```

Inline quotes with `<q>` get curly quotation marks around them: <q>inline quote</q>. You can also use the `cite` attribute on them. You can use `cite` on a `<blockquote>` too, if you enter the `<blockquote>` manually.


```
<dl>
  <dt>Publisher</dt>
  <dd>CNN and others</dd>
  <dt>Community admin</dt>
  <dd>Admins of Climate Feedback, Public Editors, etc</dd>
  <dt>Hypothesis admin</dt>
  <dt>Hypothesis developer</dt>
</dl>
```

<dl>
  <dt>Publisher</dt>
  <dd>CNN and others</dd>
  <dt>Community admin</dt>
  <dd>Admins of Climate Feedback, Public Editors, etc</dd>
  <dt>Hypothesis admin</dt>
  <dt>Hypothesis developer</dt>
</dl>




```
`<ruby>`, `<rt>` and `<rp>` can be used for [showing pronunciation of East Asian characters](http://html5doctor.com/ruby-rt-rp-element/). Example:

<ruby>
  漢 <rp>(</rp><rt>Kan</rt><rp>)</rp>
  字 <rp>(</rp><rt>ji</rt><rp>)</rp>
</ruby>
```


<ruby>
  漢 <rp>(</rp><rt>Kan</rt><rp>)</rp>
  字 <rp>(</rp><rt>ji</rt><rp>)</rp>
</ruby>

## `<div>`


```
`<div>` is also allowed, along with the `itemscope` and `itemtype` attributes for [defining microdata](http://html5doctor.com/microdata/):

<div itemscope itemtype ="http://schema.org/Movie">
  <h6 itemprop="name">Avatar</h6>
  <span>Director: <span itemprop="director">James Cameron</span> (born August 16, 1954)</span>
  <span itemprop="genre">Science fiction</span>
  <a href="https://youtu.be/0AY1XIkX7bY" itemprop="trailer">Trailer</a>
</div>
```

`<div>` is also allowed, along with the `itemscope` and `itemtype` attributes for [defining microdata](http://html5doctor.com/microdata/):

<div itemscope itemtype ="http://schema.org/Movie">
  <h6 itemprop="name">Avatar</h6>
  <span>Director: <span itemprop="director">James Cameron</span> (born August 16, 1954)</span>
  <span itemprop="genre">Science fiction</span>
  <a href="https://youtu.be/0AY1XIkX7bY" itemprop="trailer">Trailer</a>

  
  
```
HTML Entities

An `&` gets changed into `&amp;` and `<` and `>` get changed into `&lt;` and `&gt;`.
You can also enter HTML entities like `&copy;` and `&pound;` directly:
&copy;, &pound;, &sect;, &para;, &larr;, &rarr;, &hearts;.
````
  

An `&` gets changed into `&amp;` and `<` and `>` get changed into `&lt;` and `&gt;`.
You can also enter HTML entities like `&copy;` and `&pound;` directly:
&copy;, &pound;, &sect;, &para;, &larr;, &rarr;, &hearts;.

  

You can type emoji `:shortcode:`'s like `:shipit:` into the Markdown source and get an emoji like :shipit:.
See the [Emoji Cheat Sheet](https://www.webfx.com/tools/emoji-cheat-sheet/)
for the full list of emoji `:shortcode:`'s that you can use.

:bowtie:
:smile:
:laughing:
:blush:


  
  
```
  References

* [GitHub's HTML sanitization code](https://github.com/jch/html-pipeline/blob/master/lib/html/pipeline/sanitization_filter.rb#L44-L106)
* A [GitHub issue](https://github.com/github/markup/issues/245) about this
```

  
```
<ol>
  <li id="myFootnote">
    <p>
      Since you need an <code>id</code> attribute on both the footnote and on the footnote reference (to enable the footnote to contain a link <em>back</em> to the reference) I think they both need to be done in raw HTML. I don't think there's any Markdown syntax for this. See the <a href="https://gist.githubusercontent.com/seanh/13a93686bf4c2cb16e658b3cf96807f2/raw/04f35dd73445897827592a155c193976bfb756b8/Testing.markdown">source code of this file</a> for how it's done.
      <a href="#backToMyFootnote" title="Jump back to footnote 1 in the text.">↩︎</a>    
    </p>
  </li>
</ol>
```
  
<ol>
  <li id="myFootnote">
    <p>
      Since you need an <code>id</code> attribute on both the footnote and on the footnote reference (to enable the footnote to contain a link <em>back</em> to the reference) I think they both need to be done in raw HTML. I don't think there's any Markdown syntax for this. See the <a href="https://gist.githubusercontent.com/seanh/13a93686bf4c2cb16e658b3cf96807f2/raw/04f35dd73445897827592a155c193976bfb756b8/Testing.markdown">source code of this file</a> for how it's done.
      <a href="#backToMyFootnote" title="Jump back to footnote 1 in the text.">↩︎</a>    
    </p>
  </li>
</ol>



























Mon Jan 22 03:36:22 AM WET 2024
Mon Jan 22 03:46:43 AM WET 2024
Mon Jan 22 04:47:36 AM WET 2024
Mon Jan 22 04:53:07 AM WET 2024
Mon Jan 22 04:57:46 AM WET 2024
Mon Jan 22 05:29:15 AM WET 2024
