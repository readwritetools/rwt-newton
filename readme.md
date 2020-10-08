











<figure>
	<img src='/img/components/newton/paolozzi-statue-of-isaac-newton.png' width='100%' />
	<figcaption>Paolozzi statue of Isaac Newton</figcaption>
</figure>

##### Open Source DOM Component

# Newton

## Standing on the shoulders of giants


<address>
<img src='/img/rwtools.png' width=80 /> by <a href='https://readwritetools.com' title='Read Write Tools'>Read Write Tools</a> <time datetime=2020-08-02>Aug 2, 2020</time></address>



<table>
	<tr><th>Abstract</th></tr>
	<tr><td>The <span class=product>rwt-newton</span> DOM component displays document references using standardized styling.</td></tr>
</table>

#### In the wild

To see an example of this component in use, visit the <a href='https://crescentbloom.com'>Compleat Botanica</a>
website. This component typically has no visible UI. To understand what's going
on under the hood, use the browser's inspector to view the HTML source code and
network activity, and follow along as you read this documentation.

#### Prerequisites

The <span>rwt-newton</span> DOM component works in any browser that
supports modern W3C standards. Templates are written using <span>BLUE</span><span>
PHRASE</span> notation, which can be compiled into HTML using the free <a href='https://hub.readwritetools.com/desktop/rwview.blue'>Read Write View</a>
desktop app. It has no other prerequisites. Distribution and installation are
done with either NPM or via Github.

#### Installation using NPM

If you are familiar with Node.js and the `package.json` file, you'll be
comfortable installing the component just using this command:

```bash
npm install rwt-newton
```

If you are a front-end Web developer with no prior experience with NPM, follow
these general steps:

   * Install <a href='https://nodejs.org'>Node.js/NPM</a>
on your development computer.
   * Create a `package.json` file in the root of your web project using the command:
```bash
npm init
```

   * Download and install the DOM component using the command:
```bash
npm install rwt-newton
```


Important note: This DOM component uses Node.js and NPM and `package.json` as a
convenient *distribution and installation* mechanism. The DOM component itself
does not need them.

#### Installation using Github

If you are more comfortable using Github for installation, follow these steps:

   * Create a directory `node_modules` in the root of your web project.
   * Clone the <span>rwt-newton</span> DOM component into it using the command:
```bash
git clone https://github.com/readwritetools/rwt-newton.git
```


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
	<tr><td><img src='/img/read-write-hub.png' alt='DOM components logo' width=40 /></td>	<td>Documentation</td> 		<td><a href='https://hub.readwritetools.com/components/newton.blue'>READ WRITE HUB</a></td></tr>
	<tr><td><img src='/img/git.png' alt='git logo' width=40 /></td>	<td>Source code</td> 			<td><a href='https://github.com/readwritetools/rwt-newton'>github</a></td></tr>
	<tr><td><img src='/img/dom-components.png' alt='DOM components logo' width=40 /></td>	<td>Component catalog</td> 	<td><a href='https://domcomponents.com/newton.blue'>DOM COMPONENTS</a></td></tr>
	<tr><td><img src='/img/npm.png' alt='npm logo' width=40 /></td>	<td>Package installation</td> <td><a href='https://www.npmjs.com/package/rwt-newton'>npm</a></td></tr>
	<tr><td><img src='/img/read-write-stack.png' alt='Read Write Stack logo' width=40 /></td>	<td>Publication venue</td>	<td><a href='https://readwritestack.com/components/newton.blue'>READ WRITE STACK</a></td></tr>
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

