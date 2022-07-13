  

## deleting a tab "Interior" from rack
If you want to delete a tab, you can use this script
## Usage

Copy this code:
	

   
```javascript
window.onload = function () {
    try {
        var container = $('.rack').children('tbody');
        var first_value = $(container).children('tr:nth(0)');
        $(first_value).children('th:nth(2)').remove();
        var last_value = $(container).children('tr:last');
        $(last_value).children('th:nth(2)').remove();
        var current = container[0].childNodes;
        $(container).children().each(function () {
            $(this).children('td:nth(1)').remove();
        });
    }
    catch (err) {
        console.log(err);
    }
}
```


Now you can paste it into your console, for a one-time use
![enter image description here](console.png)
Console panel
