<html>
<head>
<title>Really Simple PHP Guestbook</title>
</head>
<body>
<h1 align="center">Really Simple PHP Guestbook</h1>
<div align="center">
<table border="0" cellpadding="3" cellspacing="3">
<tr><th>Name</th><th>Email</th><th>Comment</th>
</tr>
<?php
  # Guestbook file will live in the same folder with the page
  $guestbook = 'guestbook.txt';
  # Hide harmless warning messages that confuse users.
  # If you have problems and you don't know why,
  # comment this line out for a while to get more
  # information from PHP
  error_reporting (E_ALL ^ (E_NOTICE | E_WARNING));
  # Process the form submission if there is one
  if ($_POST['submit']) {
    # "a" for append
    $file = fopen($guestbook, "a");
    if (!$file) {
      echo "Can't write to guestbook file";
      die;
    }
    # Grab the form fields
    $name = $_POST['name'];
    $email = $_POST['email'];
    $comment = $_POST['comment'];
    # Remove dangerous characters, and limit the length
    $name = clean($name, 40);
    $email = clean($email, 40);
    $comment = clean($comment, 40);
    # Write a tab-delimited line to our file
    fwrite($file,
      "$date\t$name\t$email\t$comment\t$id\n");
    fclose($file);
  }
  # Now we read the file, whether we just added a line or not.
  # 'r' for read
  $file = fopen($guestbook, 'r');
  if ($file) {
    # feof is true at the end of the file, ! means not
    while (!feof($file)) {
      $line = fgets($file);
      $line = trim($line);
      # split returns an array, list re-collates the
      # array into the variables we want
      list ($name, $email, $comment) =
        split("\t", $line, 3);
      echo "<tr><td>$date</td><td>$name</td>";
      echo "<td>$email</td><td>$comment</td>";
      echo "</tr>\n";
    }
    fclose($file);
  }
  function clean($name, $max) {
    # Turn tabs and CRs into spaces so they can't
    # fake other fields or extra entries
    $name = ereg_replace("[[:space:]]", ' ', $name);
    # Escape < > and and & so they
    # can't mess withour HTML markup
    $name = ereg_replace('&', '&amp;', $name);
    $name = ereg_replace('<', '&lt;', $name);
    $name = ereg_replace('>', '&gt;', $name);
    # Don't allow excessively long entries
    $name = substr($name, 0, $max);
    return $name;
  }
?>
</table>
<form action="guestbook.php" method="POST">
<table border="0" cellpadding="5" cellspacing="5">
<tr>
<td colspan="2">Sign My Guestbook!</td>
</tr>
<tr>
<th>Name</th><td><input name="name" maxlength="40"></td>
</tr>
<tr>
<th>Email</th><td><input name="email" maxlength="40"></td>
</tr>
<tr>
<th>Comment</th><td><input name="comment" maxlength="40"></td>
</tr>
<tr>
<th colspan="2">
<input type="submit" name="submit" value="Sign the Guestbook">
</th>
</tr>
</table>
</form>
</div>
</body>
</html>
