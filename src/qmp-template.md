---
template: classless
self-contained: false
metadata:
  title: "QumaPage Sample File"
  author: 
    - name: Emanuel Regnath
      location: Germany
      email: emanuel.regnath@tum.de
  date: "2017-02-20"
  keywords: [Markdown, Example]
  bibliography: "res/bib/publications.bib"
  link-citations: yes
...


This document showcases the different things you can do.


## Feature Test
In the following, we will see how certain features are rendered.


### Math
Math is very easy to support via KaTeX.

There is inline math like $\sqrt{x^2 + \frac{1}{2}}$ and display math like

$$f_X(x)=\frac{1}{\sqrt{2\pi\sigma^2}}e^{-\frac{(x-\mu)^2}{2\sigma^2}}$$



### Boxes and Cards
To mark special content, you may use boxes. Simply start a line with `KEY:`, where `KEY` is a keyword from one of the categories:

* Hints/Examples: `Example`, `Hint`, `Tipp`
* Notes: `Note`, `Notice`, `Info`
* Warning: `Warn`, `Warning`, `Danger`, `Caution`



E.g. `Note: This is a simple note box.` produces

Note: This is a simple note box.

Example: An example.

Warn: Do not do this.




> Warning: Do not run.
> Running is too fast. 

> **Warning: Do not run.**
> Running is too fast. 


<Blockquote class="warning">

**Warning:**

Do not run.
Running is bad. 

</Blockquote>





### Simple Columns with `autorow`

:::{.autorow}

#### First Column
* A simple List
* Next item
* Another item


#### The Second Column
With Another Text

* Start of second list
* Item of second list

:::



### Hiding Details

Details: These are additional informations

A simple Q&A style unfolding is possible with `Q: / A:` syntax:

Q: What is the answer?
A: This paragraph is the answer.
The next line will also be included. 

If there is a blank line, the next paragraph is outside of the box.

#### Details: Some details page.

This is an entire section that will be hidden.

This means multiple paragraphs will disappear.

Until the next section.

##### Details: A Nested Page

More hidden content


#### Example Calculation
Uses homomorphic encryption. Works with RSA or ECC crypto.

$G ⊆ ℤ_p$ is a cyclic group, $g$ is a Generator for it.
Commitment: $H(m,r) = g^m • h^r ∈ G_p$




:::{.tabbox}

#### Case 1
With Text one.

#### Case 2
With Another Text

:::


### Figures

#### Standard Image
![Mountains as a test image from the web.](https://upload.wikimedia.org/wikipedia/commons/b/b6/Beautifull.png)


#### Tikz Image in Code Block
```{#mydia .tikz caption="Example TikZ Picture"}
\begin{tikzpicture}
\def \n {5}
\def \radius {3cm}
\def \margin {8} % margin in angles, depends on the radius

\foreach \s in {1,...,\n}
{
  \node[draw, circle] at ({360/\n * (\s - 1)}:\radius) {$\s$};
  \draw[->, >=latex] ({360/\n * (\s - 1)+\margin}:\radius)
    arc ({360/\n * (\s - 1)+\margin}:{360/\n * (\s)-\margin}:\radius);
}
\end{tikzpicture}
```

### PlantUML Test
```{.plantuml}
@startuml

VehicleModel <--up-- VehicleController: changes
VehicleModel --up--> VehicleView: notifies

VehicleView ...right...> VehicleController: (requests)

User --down--> VehicleController: requests
User <--down-- VehicleView: shows

@enduml
```



#### Plot using Plotly 
<!-- 
```{.plotly_python }
import plotly.express as px
df = px.data.iris()
fig = px.scatter(df, x="sepal_width", y="sepal_length", color="species",
                 size='petal_length', hover_data=['petal_width'])
```

 -->









### Tables


Table: Browser Support Overview.

| Name       | CSS File   | Browser Support | Dependency | License  |
|:-----------|------------|-----------------|------------|----------|
| Classless  | 400  11.2 kB | ✔ ✔ ? ✔ ✘   | none          | MIT |
| Skeleton   | 400  11.2 kB | ✔ ✔ ✔ ? ✔   | normalize     | MIT |
| Milligram  | 600  10.3 kB | ✔ ✔ ✔ ✔ ?   | normalize 8.0 | MIT |
| Sakura     | 165  3.3 kB  | ✔ ✔ ? ? ?   | (normalize)    | MIT |

Table: Browser Support Overview Caption 2.



  Right     Left     Center     Default
-------     ------ ----------   -------
     12     12        12            12
    123     123       123          123
      1     1          1             1

Table:  Demonstration of simple table syntax.


## Table Test
Bla Bla Bla
  
  Table: this is the table caption [cap]: #cap
  
  | Default | left  | Center | Right  |
  |---------|:------|:------:|-------:|
  |   High  | Cat 1 | A      | 100.00 |
  |   High  | Cat 2 | B      |  85.50 |
  |   Low   | Cat 3 | C      |  80.00 |


## Emojies and Symbols


* 🧑 Author
* 👥 Authors
* 📆 Date
* 🏆 Achievement
* 📡 Status
* 💰 Funding
* ✏ Edit
* 💡 Idea
* ⚖️ License, Terms & Conditions
* 🙏 Acknowledgment
* 📦 Packets (Software)
* 💌 Features
* 📜 Instructions
* 📚 References
* 📣 Announcements
* 🛠 Tools
* ⚙ Settings 
* 🧪 Experimental
* 🗑 Deprecated



## Inline HTML

<img height="64" src="https://latex.codecogs.com/svg.latex?f_X(x)=\frac{1}{\sqrt{2\pi\sigma^2}}e^{-\frac{(x-\mu)^2}{2\sigma^2}}">



