#form-to-firebase.html
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