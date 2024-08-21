# 0x06. Regular expression

<div class="panel panel-default">
    <div class="panel-heading">
      <h3 class="panel-title">Concepts</h3>
    </div>
    <div class="panel-body">
      <p>
        <em>For this project, we expect you to look at this concept:</em>
      </p>

<ul>
          <li>
 <a href="https://intranet.alxswe.com/concepts/29">Regular Expression</a>
          </li>
      </ul>
    </div>
  </div>

      
<h1 class="d-flex flex-column gap-2">
  <span>Regular Expression</span>
</h1>

<div>
  
</div>

<div class="gap formatted-content">
    <p>A regular expression, commonly called a &ldquo;regexp&rdquo;, is a sequence of characters that define a search pattern. &nbsp;It&nbsp;is&nbsp;mainly for use in pattern matching with strings, or string matching (i.e. it operates&nbsp;like&nbsp;a&nbsp;&ldquo;find and replace&rdquo; command). While it is a very powerful tool, it is also very dangerous because of its complexity.</p>

<p><img src="https://intranet.alxswe.com/images/contents/sysadmin/concepts/29/regex_now_2_problems.jpg" alt="" loading='lazy' style="" /></p>

<p><strong><em><a href="/rltoken/bg6ER7JUhyuRtTu9-vpQuw" title="Some people, when confronted with a problem, think" target="_blank">Some people, when confronted with a problem, think</a></em>
<em><a href="/rltoken/bg6ER7JUhyuRtTu9-vpQuw" title="“I know, I&#39;ll use regular expressions.” &nbsp; Now they have two problems." target="_blank">“I know, I&rsquo;ll use regular expressions.” &nbsp; Now they have two problems.</a></em></strong> (super classic joke in the industry)</p>

<p>One thing you have to be careful with is that different languages use different regexp engines. That&nbsp;means&nbsp;that&nbsp;a regexp in Python, for&nbsp;example,&nbsp;will be interpreted differently&nbsp;in Javascript:</p>

<p>Regular expressions are everywhere and software engineers, no&nbsp;matter their positions, will have to use them during their careers. System administrators and DevOps are the ones using them the most because&nbsp;they are very handy for log parsing.</p>

<p>Read about regexp:</p>

<ul>
<li><a href="https://www.regular-expressions.info/" title="http://www.regular-expressions.info/" target="_blank">http://www.regular-expressions.info/</a></li>
<li><p><a href="/rltoken/VOQCF4_WTOCyQ92h0dGPyA" title="https://www.w3schools.com/jsref/jsref_obj_regexp.asp" target="_blank">http://www.w3schools.com/jsref/jsref_obj_regexp.asp</a>
Play with regexp (or compose them):</p></li>
<li><p>Ruby: <a href="https://rubular.com/" title="http://rubular.com/" target="_blank">http://rubular.com/</a></p></li>
<li><p>PHP/Javascript/Python: <a href="https://regex101.com/" title="https://regex101.com/" target="_blank">https://regex101.com/</a></p></li>
</ul>

</div>


<div class="panel panel-default" id="project-description">
  <div class="panel-body">
    <h2>Background Context</h2>

<p>For this project, you have to build your regular expression using Oniguruma, a regular expression library that which is used by Ruby by default. Note that other regular expression libraries sometimes have different properties.</p>

<p>Because the focus of this exercise is to play with regular expressions (regex), here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the <code>//</code>:</p>

<pre><code>sylvain@ubuntu$ cat example.rb
#!/usr/bin/env ruby
puts ARGV[0].scan(/127.0.0.[0-9]/).join
sylvain@ubuntu$
sylvain@ubuntu$ ./example.rb 127.0.0.2
127.0.0.2
sylvain@ubuntu$ ./example.rb 127.0.0.1
127.0.0.1
sylvain@ubuntu$ ./example.rb 127.0.0.a
</code></pre>

<h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="https://www.slideshare.net/slideshow/introducing-regular-expressions/63676155" title="Regular expressions - basics" target="_blank">Regular expressions - basics</a> </li>
<li><a href="https://www.slideshare.net/slideshow/advanced-regular-expressions-80296518/80296518" title="Regular expressions - advanced" target="_blank">Regular expressions - advanced</a> </li>
<li><a href="https://rubular.com/" title="Rubular is your best friend" target="_blank">Rubular is your best friend</a> </li>
<li><a href="https://blog.codinghorror.com/regular-expressions-now-you-have-two-problems/" title="Use a regular expression against a problem: now you have 2 problems" target="_blank">Use a regular expression against a problem: now you have 2 problems</a> </li>
<li><a href="https://regexone.com/" title="Learn Regular Expressions with simple, interactive exercises" target="_blank">Learn Regular Expressions with simple, interactive exercises</a> </li>
</ul>

<h2>Requirements</h2>

<h3>General</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your files will be interpreted on Ubuntu 20.04 LTS</li>
<li>All your files should end with a new line</li>
<li>A <code>README.md</code> file, at the root of the folder of the project, is mandatory</li>
<li>All your Bash script files must be executable</li>
<li>The first line of all your Bash scripts should be exactly <code>#!/usr/bin/env ruby</code></li>
<li>All your regex must be built for the Oniguruma library</li>
</ul>

  </div>
</div>

