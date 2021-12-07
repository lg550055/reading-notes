# HTML Tables; JS Constructor Functions

## HTML Tables
As we know, tables are made of rows and columns, where each block is a cell.

#### Basic structure
> In HTML tables are written row by row.

`<table>`  -table element (whole table)
  `<tr>`   -table row element (one row)
    `<td>` -table data element (one cell)

`<th scope="col">`     -table heading (column)
`<th scope="row">`     -table heading (row)

*Use rowspan or colspan attributes to have a cell span more than one row or column*

#### Special Case: Long Tables
Long tables use three additional elements to help styling and content differentiation:
- `<thead>`
- `<tbody>`
- `<tfoot>`


---

## JS Constructor Functions
Object oriented programming uses objects to model real world things in our programs and provide a simple way to add functionality to them.

Objects can contain:
- data, which represent information and
- code, functionality about the thing you are modeling.

#### Constructors and object instances
> JavaScript uses special functions called constructor functions to define and initialize objects and their features.

**A constructor is a *function* that creates object *instances* and uses parameters to assign them *unique* property values**

***Constructors provide the means to create multiple objects efficiently***

#### Anatomy of a constructor function

function ConstuctorName(p1, p2, ) {
  this.property1 = p1;
  this.property2 = p2;
  this.action = function(){
    *function code*
  };
}

*By convention, capitalize the first letter of the constructor name*

#### Using a constructor to create an object instance
Use the keyword `new` before calling your constructor function

let instance1 = new ConstructorName(instance1par1, instance1par2);

***The beauty of constructor functions is multiple objects can be crated without the need to type each one***


---

[Back to table of contents](../README.md)