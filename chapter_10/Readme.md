Do More
======
*Use the cp -r command to copy more directories with files in them.

>Topaz-Sue:chapter_10 $ pwd
>/Users/Topaz/workspace/davinci_coders_t3_2015/homework/learn_command_line_exercises/chapter_10
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls -R
>Readme.md  orig_dir/
>
>./orig_dir:
>foo1.txt  foo2.txt
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ cp -r orig_dir/ anoth_dir
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls -R
>Readme.md  anoth_dir/ orig_dir/
>
>./anoth_dir:
>foo1.txt  foo2.txt
>
>./orig_dir:
>foo1.txt  foo2.txt
>
>(master) Sue Uyetake

*Copy a file to your home directory or desktop.
>
*Find these files in your graphical user interface and open them in a text editor.
>Yes, did so.

*Notice how sometimes I put a / (slash) at the end of a directory? That makes sure the file is really a directory, so if the directory doesn't exist I'll get an error.
>
>Topaz-Sue:chapter_10 $ pwd
>/Users/Topaz/workspace/davinci_coders_t3_2015/homework/learn_command_line_exercises/chapter_10
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls
>Readme.md  anoth_dir/ orig_dir/
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ mkdir tmp
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ touch ./tmp/foo_tmp
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ cp -r ./tmp ./third_dir
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls -R
>Readme.md  anoth_dir/ orig_dir/  third_dir/ tmp/
>
>./anoth_dir:
>foo1.txt  foo2.txt
>
>./orig_dir:
>foo1.txt  foo2.txt
>
>./third_dir:
>foo_tmp
>
>./tmp:
>foo_tmp
>
>(master) Sue Uyetake



English Questions
======
1. Can you copy the foo.txt file to slash temp? (Create foo.txt first...)
---
>
>Topaz-Sue:chapter_10 $ pwd
>/Users/Topaz/workspace/davinci_coders_t3_2015/homework/learn_command_line_exercises/chapter_10
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls
>Readme.md  anoth_dir/ orig_dir/  third_dir/ tmp/
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls tmp
>foo_tmp
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ touch foo.txt
>
>/Users/Topaz/workspace/davinci_coders_t3_2015/homework/learn_command_line_exercises/chapter_10
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls
>Readme.md  anoth_dir/ foo.txt    orig_dir/  third_dir/ tmp/
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ cp -p foo.txt /tmp
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls /tmp
>/tmp@
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ cd /tmp
>
>Topaz-Sue:tmp $ pwd
>/tmp
>
>Topaz-Sue:tmp $ ls
>4EF1BD2D-53C0-4821-B62B-E40AB481E171_IN|                KSOutOfProcessFetcher.501.I5ci1K_TwCwqo1sKvc0siaBbJTw=/
>4EF1BD2D-53C0-4821-B62B-E40AB481E171_OUT|               com.apple.launchd.4RISk2rrVB/
>EC2D9CB2-F3FC-48FE-A759-83711ACF1CE7_IN|                com.apple.launchd.d4ipcapn4g/
>EC2D9CB2-F3FC-48FE-A759-83711ACF1CE7_OUT|               foo.txt
>KSDownloadAction.LjeVL11LcF/                            log/
>KSOutOfProcessFetcher.501.HVXI9pQwBk_bgiVJaTNhiQNhqxc=/
>
>Topaz-Sue:tmp $
>

2. Can you copy .bash_profile in your home directory to the current directory?
---
>
>Topaz-Sue:chapter_10 $ pwd
>/Users/Topaz/workspace/davinci_coders_t3_2015/homework/learn_command_line_exercises/chapter_10
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls -a
>./              Readme.md       orig_dir/
>../             anoth_dir/      third_dir/
>.Readme.md.swp  foo.txt         tmp/
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ cp -p ~/.bash_profile .
>
>(master) Sue Uyetake
>Topaz-Sue:chapter_10 $ ls -a
>./              Readme.md       third_dir/
>../             anoth_dir/      tmp/
>.Readme.md.swp  foo.txt
>.bash_profile   orig_dir/
>
>(master) Sue Uyetake

#Robocopy Defined
---
>Robocopy is a windows commandline "robust copy" command that will not copy open files and is scoffed at by the book's author.

