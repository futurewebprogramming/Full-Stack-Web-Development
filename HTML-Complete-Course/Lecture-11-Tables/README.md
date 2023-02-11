# Lecture -11

### HTML Tables


HTML Tables allow us to arrange data into rows and columns

A HTML table consist table cells inside rows and columns

### Table Rows
Table Row we can add row with  
`<tr> </tr>` tags. stands for _**Table Row**_ and inside we can add our table cells.

```html
<table>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>
```

### Table Cells
table cell is defined by
`<td> cell content </td>` tag stand for _**table Data**_.

Table Cell can contain all sorts of HTML elements: like, text, images, lists, links etc..

```html
<table>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>
```

### Table Headers

Table headers used to add table headings so we use `<th>` tag stands for _**table heading**_ instead of `<td>` tag

>By default, text inside `<th>` elements are bold and centered we can change it as we want.

```html
<table>
  <tr>
    <th>Emil</th>
    <th>Tobias</th>
    <th>Linus</th>
  </tr>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>
```
### Vertical Table Headers

```html

<table>
  <tr>
    <th>Emil</th>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <th>Tobias</th>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
    <tr>
    <th>Linus</th>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>

```

### Table Borders

we can add table border as we want. we can add on `<table>` `<td> <th>`tags via css. 

```html
<style>
        table td, th{
            border: 1px solid black;

        }
</style>
```

#### Collapsed Table Borders

But as we defined table border, we will see we have double border around our table to avoid this issue. we use 

```html
<style>
        table td, th{
            border: 1px solid black;
            border-collapse: collapse;
        }
</style>
```
### Table Caption

We can Specify Table caption using `<caption>` tag.

```html

<table>
    <caption>Email Saving</caption>
  <tr>
    <th>Emil</th>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <th>Tobias</th>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
    <tr>
    <th>Linus</th>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>

```

### Padding & Spacing

Cell padding is the space between the cell edges and the cell content

```html
<style>
        td, th{
            border: 1px solid black;
            padding: 10px;
        }
</style>
```

### Table Colspan & Rowspan


#### Colspan

colspan attribute represents the number of columns to span

```html
 <table>
        <caption>Result Table</caption>
            <tr>
                <th colspan="2">Name</th>
                <th>Class</th>
                <th>Rank</th>
                <th>Obtained Marks</th>
                <th>Total Marks</th>
            </tr>
            <tr>
                <td>Future</td>
                <td>Programing</td>
                <td >MS</td>
                <td>A++</td>
                <td>450</td>
                <td>500</td>
            </tr>
    </table>
```
<table>
        <caption>Result Table</caption>
            <tr>
                <th colspan="2">Name</th>
                <th>Class</th>
                <th>Rank</th>
                <th>Obtained Marks</th>
                <th>Total Marks</th>
            </tr>
            <tr>
                <td>Future</td>
                <td>Programing</td>
                <td >MS</td>
                <td>A++</td>
                <td>450</td>
                <td>500</td>
            </tr>
    </table>

### Rowspan

Span cell over multiple rows

```html
 <table>
        <tr>
            <th rowspan="2">Name</th>
            <td>Future</td>
        </tr>
        <tr>
            <td>Programming</td>
        </tr>
        <tr> 
            <th rowspan="2">Class</th>
            <td>MS</td>
        </tr>
        <tr>
            <td>MSc</td>
        </tr>
        <tr>
            <th>Roll Number</th>
            <td>1</td>
        </tr>
    </table>
```

 <table>
        <tr>
            <th rowspan="2">Name</th>
            <td>Future</td>
        </tr>
        <tr>
            <td>Programming</td>
        </tr>
        <tr> 
            <th rowspan="2">Class</th>
            <td>MS</td>
        </tr>
        <tr>
            <td>MSc</td>
        </tr>
        <tr>
            <th>Roll Number</th>
            <td>1</td>
        </tr>
    </table>
    
#### Table Colgroup

Colgroup tag used to style specific columns of a table

```html
 <colgroup>
            <col span="2">
            <col span="1" style="background-color: yellow;">
            <col span="1" style="background-color: darkblue;">
        </colgroup>

```

#### Table Styling
#### Zebra Stripes effect

>add a background color on every other table row, you will get a nice zebra stripes effect

>To style every other table row element, use the :nth-child(even)

We will cover Table Styling in CSS Module. 
