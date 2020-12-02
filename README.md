# FILE UPLOAD SYSTEM:<br>
:white_circle: **File upload করার জন্য যাযা করণীয়:**<br>
- প্রথমে Form crate করতে হবে। Then Form enctype="multipart/form-data” type দিতেই হবে ।
- Input a data দিয়ে submit করে data ধরতে হবে । Data ধরার সময় input name এ  $_GET/$_POST এর পরিবতে, $_FILES['name']; দিতে হবে ।<br>
:star: **EXEMPLE**: $photo = $_FILES['picter'];<br>
- এর পরে file upload করার জন্য move_uploaded_file($tmp_name ,'images/'.$newName); লিখতে হবে । <br><br>
:star: **NOTE:** $tmp_name= tmp_name/con নাম/কানেকশন।<br>
:star: **NOTE:** 'images/'= directory file location কোন জায়গায়/folder এ file save হবে ।<br>
:star: **NOTE:**.$newName= File new name/extention কি হবে ।<br><br>
- এর পরে Validation করে File Upload করতে পারি । 
