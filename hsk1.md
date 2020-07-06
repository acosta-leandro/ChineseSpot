---
title: HSK-1
subtitle: Words from HSK1
layout: "post"
icon: fa-book
order: 4
---
<hr>
	<header>
		<h2>HSK 1</h2>
		<p>Ordered by phonetics</p>
	</header>
	<p>These files have been generated from the latest (as of November 2013) which word lists published by Hanban in September 2012</p>
<hr />

<h2>Text</h2>
<p>This is <b>bold</b> and this is <strong>strong</strong>. This is <i>italic</i> and this is <em>emphasized</em>.
	This is <sup>superscript</sup> text and this is <sub>subscript</sub> text.
	This is <u>underlined</u> and this is code: <code>for (;;) { ... }</code>.
	Finally, this is a <a href="#">link</a>.</p>
	<hr />
	<h2>Heading Level 2</h2>
	<h3>Heading Level 3</h3>
	<hr />
	<header>
		<h2>Heading with a Subtitle</h2>
		<p>Lorem ipsum dolor sit amet nullam id egestas urna aliquam</p>
	</header>
	<p>Nunc lacinia ante nunc ac lobortis. Interdum adipiscing gravida odio porttitor sem non mi integer non faucibus ornare mi ut ante amet placerat aliquet. Volutpat eu sed ante lacinia sapien lorem accumsan varius montes viverra nibh in adipiscing blandit tempus accumsan.</p>
	<hr />

<table>
  {% for row in site.data.hsk1 %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>