form-to-firebase.html
Just name a class to your form and form submit to firebase

<script>
$('.firebaseajax').submit(function(e) {
  // $("#loader").removeClass("d-none");
  e.preventDefault();
  // $(this).append('<input type="hidden" name="newAttribute" value="newValue">');

  output = $.fn.formToFirebase(this,'no','no');
  output.then(function(data) {
    // handle success
    console.log(data);
    // $("#loader").addClass("d-none");
  }).catch(e => {
    // handle catch
    console.log(e);
    // $("#loader").addClass("d-none");
  });
});
</script>#   f i r e b a s e - f u n c t i o n s  
 