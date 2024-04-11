## limitations
Realtime database only

## things to cover
Following points are remaing
- Add picture upload + retrive
- Orderby
- Pagination
- records per page
- records counting
- loader - i think no need
- when new record added please record not clearing

# form-to-firebase.html
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

# firebase-to-table.html
Check the file
```
Call the function
<script>
$.fn.firebaseToTable('.firebase-to-table');
</script>
```

# firebase-to-div.html
Check the file
```
Call the function
<script>
$.fn.firebaseToDiv('.firebase-to-div');
</script>
```

