<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
</head>
<body>

<div id="demo">
<h2>The XMLHttpRequest Object</h2>
<button type="button" onclick="httpGet()">Change Content</button>
</div>
<script>
$.ajax({
    url: 'https://docs.google.com/spreadsheets/d/e/2PACX-1vQuDj0R6K85sdtI8I-Tc7RCx8CnIxKUQue0TCUdrFOKDw9G3JRtGhl64laDd3apApEvIJTdPFJ9fEUL/pubhtml?gid=0&single=true&fbclid=IwAR3czc19tmrX0FhxoxbjH6-0DgdOzetPOr__rdXN59-VlqWgWbgjFvCQ5QM',
    headers: { 'Content-Type': 'application/json'},
    type: "GET", /* or type:"GET" or type:"PUT" */
    dataType: "jsonp",
    data: {
    },
    success: function (result) {
        console.log(result);
    },
    error: function () {
        console.log("error");
    }
});

  
</script>

</body>
</html>


