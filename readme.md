












<figure>
	<img src='/img/components/newton/newton-1500x750.png' width='100%' />
	<figcaption>Paolozzi statue of Isaac Newton</figcaption>
</figure>

##### Open Source DOM Component

# Newton

## Standing on the shoulders of giants


<address>
<img src='/img/48x48/rwtools.png' /> by <a href='https://readwritetools.com' title='Read Write Tools'>Read Write Tools</a> <time datetime=2020-08-02>Aug 2, 2020</time></address>



<table>
	<tr><th>Abstract</th></tr>
	<tr><td>The <span class=product>rwt-newton</span> DOM component displays document references using standardized styling.</td></tr>
</table>

#### In the wild

To see an example of this component in use, visit the <a href='https://crescentbloom.com'>Compleat Botanica</a>
website. This component typically has no visible UI. To understand what's going
on under the hood, use the browser's inspector to view the HTML source code and
network activity, and follow along as you read this documentation.

### Installation

#### Prerequisites

The <span>rwt-newton</span> DOM component works in any browser that
supports modern W3C standards. Templates are written using <span>BLUE</span><span>
PHRASE</span> notation, which can be compiled into HTML using the free <a href='https://hub.readwritetools.com/desktop/rwview.blue'>Read Write View</a>
desktop app. It has no other prerequisites. Distribution and installation are
done with either NPM or via Github.

#### Download


<details>
	<summary>Download using NPM</summary>
	<p><b>OPTION 1:</b> Familiar with Node.js and the <code>package.json</code> file?<br />Great. Install the component with this command:</p>
	<pre lang=bash>
npm install rwt-newton<br />	</pre>
	<p><b>OPTION 2:</b> No prior experience using NPM?<br />Just follow these general steps:</p>
	<ul>
		<li>Install <a href='https://nodejs.org'>Node.js/NPM</a> on your development computer.</li>
		<li>Create a <code>package.json</code> file in the root of your web project using the command:</li>
		<pre lang=bash>
npm init<br />		</pre>
		<li>Download and install the DOM component using the command:</li>
		<pre lang=bash>
npm install rwt-newton<br />		</pre>
	</ul>
	<p style='font-size:0.9em'>Important note: This DOM component uses Node.js and NPM and <code>package.json</code> as a convenient <i>distribution and installation</i> mechanism. The DOM component itself does not need them.</p>
</details>


<details>
	<summary>Download using Github</summary>
	<p>If you prefer using Github directly, simply follow these steps:</p>
	<ul>
		<li>Create a <code>node_modules</code> directory in the root of your web project.</li>
		<li>Clone the <span class=product>rwt-newton</span> DOM component into it using the command:</li>
		<pre lang=bash>
git clone https://github.com/readwritetools/rwt-newton.git<br />		</pre>
	</ul>
</details>

### Using the DOM component

After installation, you need to add two things to your HTML page to make use of
it.

   * Add a `script` tag to load the component's `rwt-newton.js` file:
```html
<script src='/node_modules/rwt-newton/rwt-newton.js' type=module></script>             
```

   * Add the component tag somewhere on the page, supplying four pieces of slotted
      text:

      1. `span slot=h2` The h2 heading text (optional).
      2. `span slot=h3` The h3 heading text (optional).
      3. `span slot=dt` A definition term.
      4. `span slot=dd` A definition description. This typically has an anchor tag with the
         external reference.

Here's an example:

```html
<rwt-newton role=navigation>
    <span slot=h2>Giants</span>
    <span slot=h3>Isaac Newton</span>
    <span slot=dt>Famous quotes</span>
    <span slot=dd><a href='https://example.com/shoulders-of-giants.html'> If I Have Seen Further</a> Using the understanding gained by major thinkers who have gone before in order to make intellectual progress.</span>
</rwt-newton>
```

### Customization

The reference area has limited customization. Only the background color may be
customized. Supply a background color using the `background` attribute.

```html
<rwt-newton role=navigation background='#777'>
    ...
</rwt-newton>
```

### Life-cycle events

The component issues life-cycle events.


<dl>
	<dt><code>component-loaded</code></dt>
	<dd>Sent when the component is fully loaded and ready to be used. As a convenience you can use the <code>waitOnLoading()</code> method which returns a promise that resolves when the <code>component-loaded</code> event is received. Call this asynchronously with <code>await</code>.</dd>
</dl>

---

### Reference


<table>
	<tr><td><img src='/img/48x48/read-write-hub.png' alt='DOM components logo' width=48 /></td>	<td>Documentation</td> 		<td><a href='https://hub.readwritetools.com/components/newton.blue'>READ WRITE HUB</a></td></tr>
	<tr><td><img src='/img/48x48/git.png' alt='git logo' width=48 /></td>	<td>Source code</td> 			<td><a href='https://github.com/readwritetools/rwt-newton'>github</a></td></tr>
	<tr><td><img src='/img/48x48/dom-components.png' alt='DOM components logo' width=48 /></td>	<td>Component catalog</td> 	<td><a href='https://domcomponents.com/components/newton.blue'>DOM COMPONENTS</a></td></tr>
	<tr><td><img src='/img/48x48/npm.png' alt='npm logo' width=48 /></td>	<td>Package installation</td> <td><a href='https://www.npmjs.com/package/rwt-newton'>npm</a></td></tr>
	<tr><td><img src='/img/48x48/read-write-stack.png' alt='Read Write Stack logo' width=48 /></td>	<td>Publication venue</td>	<td><a href='https://readwritestack.com/components/newton.blue'>READ WRITE STACK</a></td></tr>
</table>

### License

The <span>rwt-newton</span> DOM component is licensed under the MIT
License.

<img src='/img/blue-seal-mit.png' width=80 align=right />

<details>
	<summary>MIT License</summary>
	<p>Copyright © 2020 Read Write Tools.</p>
	<p>Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:</p>
	<p>The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.</p>
	<p>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</p>
</details>

