# xclip

> أداة معالجة لحافظة x11، تشبه إلي حد ما `xsel`.
> تتعامل مع الحافظة الأولية والثانوية لـ x، بالإضافة إلي حافظة النظام (`<Ctrl c>`/`<Ctrl v>`).
> لمزيد من التفاصيل: <https://manned.org/xclip>.

- إنسخ ناتج الخرج من أمر إلي حافظة x11 الأولية:

`echo 123 | xclip`

- إنسخ ناتج الخرج من أمر إلي الحافظة المختارة:

`echo 123 | xclip -selection {{primary|secondary|clipboard}}`

- إنسخ ناتج الخرج من أمر إلي حافظة النظام، باستخدام الصيغة المختصرة:

`echo 123 | xclip -sel clip`

- إنسخ محتوي ملف إلي حافظة النظام:

`xclip -sel clip {{input_file.txt}}`

- إنسخ محتوي صورة بصيغة PNG إلي حافظة النظام (يمكن أن تستخدم في أي برنامج عن طريق لصق):

`xclip -sel clip -t image/png {{input_file.png}}`

- إنسخ إدخال المستخدم في الطرفية أو الكونسول إلي حافظة النظام:

`xclip -i`

- إلصق محتوي حافظة x11 الأولية إلي الطرفية أو الكونسول:

`xclip -o`

- إلصق محتوي حافظة النظام إلي الطرفية أو الكونسول:

`xclip -o -sel clip`
