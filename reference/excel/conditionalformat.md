# ConditionalFormat Object (JavaScript API for Excel)

An object encapsulating a conditional format's range, format, rule, and other properties.

## Properties

| Property	   | Type	|Description| Req. Set|
|:---------------|:--------|:----------|:----|
|id|string|The Priority of the Conditional Format within the current ConditionalFormatCollection. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|priority|int|The priority (or index) within the conditional format collection that this conditional format currently exists in. Changing this also|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|stopIfTrue|bool|If the conditions of this conditional format are met, no lower-priority formats shall take effect on that cell.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|type|string|A type of conditional format. Only one can be set at a time. Read-only. Possible values are: Custom, DataBar, ColorScale, IconSet.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|

_See property access [examples.](#property-access-examples)_

## Relationships
| Relationship | Type	|Description| Req. Set|
|:---------------|:--------|:----------|:----|
|cellValue|[CellValueConditionalFormat](cellvalueconditionalformat.md)|Returns the cell value conditional format properties if the current conditional format is a CellValue type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|cellValueOrNullObject|[CellValueConditionalFormat](cellvalueconditionalformat.md)|Returns the cell value conditional format properties if the current conditional format is a CellValue type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|colorScale|[ColorScaleConditionalFormat](colorscaleconditionalformat.md)|Returns the ColorScale conditional format properties if the current conditional format is an ColorScale type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|colorScaleOrNullObject|[ColorScaleConditionalFormat](colorscaleconditionalformat.md)|Returns the ColorScale conditional format properties if the current conditional format is an ColorScale type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|custom|[CustomConditionalFormat](customconditionalformat.md)|Returns the custom conditional format properties if the current conditional format is a custom type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|customOrNullObject|[CustomConditionalFormat](customconditionalformat.md)|Returns the custom conditional format properties if the current conditional format is a custom type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|dataBar|[DataBarConditionalFormat](databarconditionalformat.md)|Returns the data bar properties if the current conditional format is a data bar. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|dataBarOrNullObject|[DataBarConditionalFormat](databarconditionalformat.md)|Returns the data bar properties if the current conditional format is a data bar. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|iconSet|[IconSetConditionalFormat](iconsetconditionalformat.md)|Returns the IconSet conditional format properties if the current conditional format is an IconSet type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|iconSetOrNullObject|[IconSetConditionalFormat](iconsetconditionalformat.md)|Returns the IconSet conditional format properties if the current conditional format is an IconSet type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|preset|string|Returns the preset criteria conditional format. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|presetOrNullObject|string|Returns the preset criteria conditional format. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|textComparison|[TextConditionalFormat](textconditionalformat.md)|Returns the specific text conditional format properties if the current conditional format is a text type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|textComparisonOrNullObject|[TextConditionalFormat](textconditionalformat.md)|Returns the specific text conditional format properties if the current conditional format is a text type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|topBottom|[TopBottomConditionalFormat](topbottomconditionalformat.md)|Returns the TopBottom conditional format properties if the current conditional format is an TopBottom type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|topBottomOrNullObject|[TopBottomConditionalFormat](topbottomconditionalformat.md)|Returns the TopBottom conditional format properties if the current conditional format is an TopBottom type. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|

## Methods

| Method		   | Return Type	|Description| Req. Set|
|:---------------|:--------|:----------|:----|
|[delete()](#delete)|void|Deletes this conditional format.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|[getRange()](#getrange)|[Range](range.md)|Returns the range the conditonal format is applied to. Throws an error if the conditional format is applied to multiple ranges. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|[getRangeOrNullObject()](#getrangeornullobject)|[Range](range.md)|Returns the range the conditonal format is applied to, or a null object if the conditional format is applied to multiple ranges. Read-only.|[1.6](../requirement-sets/excel-api-requirement-sets.md)|
|[getRanges()](#getranges)|[RangeAreas](rangeareas.md)|Returns the RangeAreas, comprising one or more rectangular ranges, the conditonal format is applied to. Read-only.|[beta](../requirement-sets/excel-api-requirement-sets.md)|

## Method Details


### delete()
Deletes this conditional format.

#### Syntax
```js
conditionalFormatObject.delete();
```

#### Parameters
None

#### Returns
void

### getRange()
Returns the range the conditonal format is applied to. Throws an error if the conditional format is applied to multiple ranges. Read-only.

#### Syntax
```js
conditionalFormatObject.getRange();
```

#### Parameters
None

#### Returns
[Range](range.md)

### getRangeOrNullObject()
Returns the range the conditonal format is applied to, or a null object if the conditional format is applied to multiple ranges. Read-only.

#### Syntax
```js
conditionalFormatObject.getRangeOrNullObject();
```

#### Parameters
None

#### Returns
[Range](range.md)

### getRanges()
Returns the RangeAreas, comprising one or more rectangular ranges, the conditonal format is applied to. Read-only.

#### Syntax
```js
conditionalFormatObject.getRanges();
```

#### Parameters
None

#### Returns
[RangeAreas](rangeareas.md)
### Property access examples
