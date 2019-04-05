## Text Field

This sub directory contains UI code samples for working with text fields.

Displays a text field to capture an text input.

**Attributes:**
  1) **css** - Any css classes to be applied

      **values** - text

**Inner Nodes:**
  1) **Footer** - Display helper text beside the text field

#### FieldLine

Used to line-up fields horizontally. Internally, this wraps fields in a span tag (as opposed to FieldBlock elements that wrap fields in div tags). When alignment is specified, elements are wrapped in a div tag. Use this to center/right align elements in a horizontal fashion.

**Attributes:**
  1) **align** - Align the fields accordingly
  
      **values** - right | left | center

  2) **title.css** - Any css classes to be applied
  
      **values** - text

#### Sample

![Text Field](images/s1.PNG)