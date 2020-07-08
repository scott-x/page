# page
100% native JS plugin for pagnation

### how to use
```html
<!DOCTYPE HTML>
<html lang="en-US">
<head>
	<meta charset="UTF-8">
	<title>pagnation plugin</title>
  <link rel="stylesheet" href="custom-pagination.min.css" /><!-- 1.import css -->
  <style type="text/css">
    html,body{
      width: 100%;
      height: 100%;
      margin: 0;
      padding: 0;
      border: 0;
    }
    #page{
      width: 100%;
      height: 80px;
      margin: 50px 0;
    }
  </style>
</head>
<body>
  <div id="page" class="page"></div><!-- 2.create a page container，and set up the width -->
  
	<script type="text/javascript" src="custom-pagination.min.js"></script><!-- 3.importjs -->
  <script type="text/javascript">
    // 4. use the plugin
    var box = new CustomPagination('#page', {
      total: 100,//total pages
      changePage: function (pageNum) {
        //when page chaned
        //code...
        console.log('current page:'+pageNum)
      }
    });
  </script>
</body>
</html>
```