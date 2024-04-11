#
form-to-firebase.html
#
Just name a class to your form and form submit to firebase
```
<script>
$('.firebaseajax').submit(function(e) {
  e.preventDefault();
  output = $.fn.formToFirebase(this,'no','no');
  output.then(function(data) {
    // handle success
    console.log(data);
  }).catch(e => {
    // handle catch
    console.log(e);
  });
});
</script>
```

#
firebase-to-table.html
#
Just name a class to your table and add data attbiute to your table td

```
Html work inside table element
<table class="firebase-to-table" data-ref="reviews">

Html work for td inside tbody
<td data-col="name"></td>
<td data-col="review"></td>

Call the function
<script>
$.fn.firebaseToTable('.firebase-to-table');
</script>
```