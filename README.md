| :warning: DISCLAIMER          |
|:---------------------------|
| This plugin is currently in testing phase. This might be not working in some use-cases. If you face any issue Please let us know, any kind of feedbac would be appreciated.      |

# Future dates

This is a basic Jquery plugin that might be helpful in your following use-cases.

- In order to get only future dates. E.g. I want to get next 10 dates, next 2 weeks dates, etc.
- you can set your desired date format.

# Dependencies
- Jquery ( v3.1 or greater)



# Getting Started

Download the file `futureDates.min.js`


- include jquery libray.
```javascript
  <script type="text/javascript" src="jquery-3.3.1.js"></script>
```

- include `futureDates.min.js` that you have Downloaded.
```javascript
  <script type="text/javascript" src="/path/to/futureDates.min.js"></script>
```
- Its done and ready to use.

```javascript
$(document).ready(function(){
    # example 1
    var futureDates = FutureDates();
    // open browser console to see results.
    console.log(futureDates);
    
    # example 1
    var futureDates2 = FutureDates({
                          dateFormat:'dd/mm/yyyy', 
                          noOfFutureDates:25,
                        });
    // open browser console to see results.
    console.log(futureDates2);
});  
```

- Above use-case will gives you results in array. By default, There'll future 28 dates in `mm/dd/yyy` date format.

# Options

| Property | Type | DefaultValue | Description
| -------- | -----| ------------ | -----------
| dateFormat  | string | `mm/dd/yyyy`  | `null`
| noOfFutureDates  | string/integers | 28  | `null`
| includeToday  | boolean(TRUE,FALSE,1,0) | false  | `null`
| endDate  | string, date format `mm/dd/yyy` | undefined  | `endDate` will override `noOfFutureDates`

## DateFormat Options

| dateFormat | Result 
| ---------- | ----- |
| `mm/dd/yyyy` | `02/21/2018` |
| `mm/dd/yy` | `02/21/18`
| `dd/mm/yyyy` | `21/02/2018`
| `dd/mm/yy` | `21/02/18`
| `dd-mm-yyyy` | `21-02-2018`
| `dd-mm-yy` | `21-02-18`
| `mm-dd-yyyy` | `02-21-2018`
| `mm-dd-yy` | `02-21-18`
| `yyyy-mm-dd` | `2018-02-21`
| `m/d/yyyy` | `2/21/2018`
| `m/d/yy` | `2/21/18`
| `d/m/yyyy` | `21/2/2018`
| `d/m/yy` | `21/2/18`
| `m-d-yyyy` | `2-21-2018`
| `m-d-yy` | `2-21-18`
| `d-m-yyyy` | `21-2-2018`
| `d-m-yy` | `21-2-18`
| `Mth d, yyyy` | `Feb 21, 2018`
| `Month d, yyyy` | `February 21, 2018`



## Thanks

**Any feedback or ideas will be highly appreciated.**
Thanks :) 
    
