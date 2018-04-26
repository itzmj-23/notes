# notes
my notes for development, it may be useful sometimes when I forget something, so I try to look for it here if I already done it before.

## PHP

### empty
I encounted in `<input type="number">` that even the field is empty, the `empty()` is not returning `true`;

I have found it in [Stackoverflow](https://stackoverflow.com/questions/2216052/how-to-check-whether-an-array-is-empty-using-php).
```
$quantity = $_POST['quantity'];
foreach ($quantity as $key => $value) {
  if (empty($value)) {
     unset($quantity[$key]);
  }
}
if(!empty($quantity)){
  echo 'not empty';
} else {
  echo 'empty';
}
```

### get form input array into PHP array
[Stackoverflow](https://stackoverflow.com/questions/3314567/how-to-get-form-input-array-into-php-array)

