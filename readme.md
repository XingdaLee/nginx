```
"reload": "nginx -s reload",
"start": "start nginx"
```

``E:\Codes\nginx``

```
  var requestJson = {
    "activity_status": '1'
  };
  $.ajax({
    type: "post",
    contentType: "application/json",
    url: "/test/find_activity_list",
    dataType: "json",
    data: JSON.stringify(requestJson),
    success: function (brand_data) {
      renderList(brand_data)
    },
    error: function (XMLHttpRequest, textStatus, errorThrown) {

    }
  });
```