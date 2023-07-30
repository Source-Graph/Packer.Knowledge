# HereDoc
## Indented:
>To improve on this, Packer also accepts an indented heredoc string variant that is introduced by the <<- sequence:
>```
>block {
>  value = <<-EOF
>  hello
>    world
>  EOF
>}
>```
>
>In this case, Packer analyses the lines in the sequence to find the one with the smallest number of leading spaces, and then trims that many spaces from the beginning of all of the lines, leading to the following result:
>```
>hello
>  world
>```
