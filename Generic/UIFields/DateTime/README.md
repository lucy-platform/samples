## Date Time

This sub directory contains UI code samples for working with date time UI fields.

Shows a field to select a date and time. This field will show a date control with a popup calendar to pick a date as well as a time control to enter or select a time. The value you assign to this field must be a datetime value and must be in UTC. You can set which timezone to render the datetime value in by assigning the timezone attribute. When reading the value on the server using `#{field.id}` it will return the value in UTC. You can access the timezone that was used in the UI by reading `#{field.id__tz}`.

**Attributes:**
  1) **dateonly** - If set to true, then the time component is hidden and assumed to be *00:00* in the assigned timezone (**NOT** in *UTC* timezone)
  
      **values** - true | false
  
  2) **can_clear** - Set to true to allow the field to be cleared by clicking the **X**. When cleared, reading #{field.id} will return null. Set to false to prevent it from being cleared. Note that even if you set this to false, you still need to check for null in the backend because the its possible the field was empty when it loaded. (If the value assigned was empty).
  
      **values** - true | false
  
  3) **timezone** - Specify the timezone that this field should render in. The timezone will be shown next to the datetime control

      **values** - text

  4) **value** - The value to assign to the field. It must be a datetime object in UTC. If you want to assign it from a text string (like a query string parameter) then convert the text string to a datetime object using the `|datetime` _transformer_

      ```
      Example: value='#{param.starts|datetime}'
      Example: value='#{[20190405:112800]|datetime}'
      ```

      **Note:** The text must be in the form yyyMMdd:HHmmss OR yyyyMMdd

      **values** - datetime

#### Sample

![Date Time Fields](images/s1.PNG)

#### Illustration

![Illustration](images/s2.gif)